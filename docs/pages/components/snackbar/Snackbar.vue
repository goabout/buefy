<template>
    <div>
        <div class="content">
            <p>They have only one button, and by default are queued to not confuse the user.</p>
            <p><small><b>Note:</b> They queue with <router-link to="/documentation/toast">Toasts</router-link> as well.</small></p>
            <div class="tags has-addons">
                <span class="tag is-success">New!</span>
                <span class="tag is-info">0.6.2</span>
            </div>
            <p>
                You can disable queue by passing the <code>queue: false</code> object attribute or by using
                <router-link to="/documentation/constructor-options">constructor options</router-link>.
            </p>
        </div>

        <Example :component="ExSimple" :code="ExSimpleCode"/>

        <ApiView :data="api"/>
    </div>
</template>

<script>
    import api from './api/snackbar'

    import ExSimple from './examples/ExSimple'
    import ExSimpleCode from '!!raw-loader!./examples/ExSimple'

    export default {
        data() {
            return {
                api,
                ExSimple,
                ExSimpleCode
            }
        }
    }
</script>

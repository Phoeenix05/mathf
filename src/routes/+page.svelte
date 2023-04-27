<script lang="ts">
    import { Notification } from '@svelteuidev/core';

    let notif_visible = true;
</script>

{#if notif_visible}
    <Notification title="Note" color="red" on:close={() => notif_visible = false}>
        This application will only work in finland unless there are some apis I can use to get tax procentages.
    </Notification>
{/if}

<a href="/exchange/stock">Stock</a>
<br>
<a href="/tax/inheritance">Inheritance tax</a>
<br>
<p>Home</p>
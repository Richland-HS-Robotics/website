<script>
    export let items = [];
    export let activeTabValue = 1;

    const handleClick = (tabValue) => () => (activeTabValue = tabValue);
</script>

<div class="bg">
    <ul>
        {#each items as item}
            <li class={activeTabValue === item.value ? "active" : ""}>
                <span on:click={handleClick(item.value)}>{item.label}</span>
            </li>
        {/each}
    </ul>


    {#if activeTabValue == 1}
        <div class="box"> <slot name="body1"></slot> </div>
    {/if}
    {#if activeTabValue == 2}
        <div class="box"> <slot name="body2"></slot> </div>
    {/if}
    {#if activeTabValue == 3}
        <div class="box"> <slot name="body3"></slot> </div>
    {/if}
</div>

<style>
    .bg {
        background-color: var(--bg-color);
    }
    .box {
        border: 1px solid var(--yellow);
        border-radius: 7px;
        width: 90vw;
        background-color: var(--secondary-bg-color);
        color: var(--text-color);
        margin-left: 0;
        box-shadow: 0 0 15px var(--secondary-bg-color);
    }
    ul {
        display: flex;
        flex-wrap: wrap;
        padding-left: 0;
        margin-bottom: 20px;
        margin-left: -15px;
        list-style: none;
        padding-top: 20px;
    }
    li {
        margin-bottom: -1px;
    }

    span {
        border: 0;
        border-radius: 7px;
        cursor: pointer;
        display: inline-block;
        height: 3.25rem;
        line-height: 3.25rem;
        padding: 0 20px;
        text-align: center;
        text-decoration: none;
        white-space: nowrap;
        font-size: 20px;
        margin-left: 10px;
        margin-right: 10px;
        background-color: var(--secondary-bg-color);
        border: 2px solid var(--green);
        color: var(--text-color);
    }

    span:hover {
        border-color: var(--green-hover);
    }

    li.active > span {
        border: 0;
        border-radius: 7px;
        cursor: default;
        display: inline-block;
        height: 3.25rem;
        line-height: 3.25rem;
        padding: 0 20px;
        text-align: center;
        text-decoration: none;
        white-space: nowrap;
        font-size: 20px;
        background: linear-gradient(0deg, hsl(42 100% 50%), var(--yellow));
        box-shadow: 0 0 15px var(--yellow);
        color: var(--bg-color);
    }
</style>

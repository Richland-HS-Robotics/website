<div class="bg">
    <div class="left">
        <slot name="left"></slot>
    </div>
    <div class="right">
        <slot name="right"></slot>
    </div>
</div>


<link
    href="https://fonts.googleapis.com/css?family=Open+Sans"
    rel="stylesheet"
/>

<style>
    .bg {
        background-color: var(--bg-color);
        width: 100%;
        display: flex;
        padding-top: 25px;
        z-index: 0;
    }
    .left {
        width: 40vw;
        margin-left: 0;
        z-index: 2;
    }
    .right {
        width: 50%;
        margin-right: 5vw;
        z-index: 2;
    }
    @media only screen and (max-width: 768px) {
        .left {
            width: 90vw;
            order: 1;
        }
        .bg {
            flex-direction: column;
            padding-top: 50px;
        }
        .right {
            width: 90vw;
            margin-left: 0;
            margin-right: 0;
            order: 0;
        }
    }
</style>

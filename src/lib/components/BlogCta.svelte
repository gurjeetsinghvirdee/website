<script lang="ts">
    export let heading: string = 'Start building with Appwrite today';
    export let url: string = 'https://cloud.appwrite.io';
    export let label: string = 'Get started';
</script>

<div
    class="bg relative mt-12 !-mb-28 flex min-h-[12rem] items-center justify-center overflow-hidden border-t border-[hsl(var(--web-color-subtle))] py-12 lg:!-mb-[64px]"
>
    <div class="flex max-w-3xs flex-col items-center justify-center gap-5 text-center">
        <h2 class="text-label text-primary font-aeonik-pro">{heading}</h2>
        <a href={url} class="web-button">{label}</a>
    </div>
</div>

<style lang="scss">
    .bg {
        &::before {
            content: '';
            position: absolute;
            inset: 0;
            height: 170%;
            z-index: -1;
            background-image: radial-gradient(
                ellipse at center,
                rgba(253, 54, 110, 0.09),
                transparent 85%
            );
        }
    }
</style>

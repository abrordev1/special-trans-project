<template>
    <div class="card border border-light-gray rounded-lg p-5 flex items-center gap-3 w-full">
        <div class="icon">
            <slot name="icon" />
        </div>
        <div class="text text-sm text-dark">
            <slot name="text" />
        </div>
    </div>
</template>  
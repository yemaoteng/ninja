<template>
    <div>
        <slot name="form-header"></slot>
        <slot name="form-p"></slot>
        <label for="name">Name:</label>
        <input type="text" name="name" placeholder="Please enter your name" />
        <label for="phone">Phone</label>
        <input type="text" name="phone" />
        <slot name="form-footer"></slot>
    </div>
</template>

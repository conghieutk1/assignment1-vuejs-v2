<template>
    <button class="r-btn">{{ nameTab }}</button>
</template>

<script>
export default {
    mounted() {
        var buttons = document.querySelectorAll('.r-btn');
        Array.prototype.forEach.call(buttons, function (b) {
            b.addEventListener('click', createRipple);
        });
        function createRipple(event) {
            var ripple = document.createElement('span');
            ripple.classList.add('ripple');
            var max = Math.max(this.offsetWidth, this.offsetHeight);
            ripple.style.width = ripple.style.height = max * 2 + 'px';
            var rect = this.getBoundingClientRect();
            ripple.style.left = event.clientX - rect.left - max + 'px';
            ripple.style.top = event.clientY - rect.top - max + 'px';
            this.appendChild(ripple);
            // Remove the ripple after animation completes
            ripple.addEventListener('animationend', () => {
                ripple.remove();
            });
        }
    },
    props: ['nameTab'],
};
</script>

<style lang="scss" scoped>
button {
    font-family: 'Satoshi', sans-serif;
    font-size: 16px;
    font-weight: 400;
    line-height: 21.6px;
    text-align: left;
    white-space: nowrap;
    cursor: pointer;
    margin: 10px 0px;
    position: relative;
    overflow: hidden;
    padding: 10px 15px;
    background-color: transparent;
    border: none;
    outline: none !important;
    color: black !important;
    transition: 0.1s;
    &::before {
        content: '';
        height: 3px;
        width: 0;
        left: 0;
        bottom: 0;
        position: absolute;
        background: black;
        transition: 0.4s;
    }
    &:hover {
        &::before {
            width: 100%;
        }
    }
    &:active {
        background-color: rgba(255, 255, 255, 0.1);
    }
}

:deep(span.ripple) {
    background-color: gray;
    opacity: 40%;
    border-radius: 50%;
    position: absolute;
    transform: scale(0);
    animation: ripple 0.4s linear forwards;
    @keyframes ripple {
        to {
            transform: scale(1);
            opacity: 0;
        }
    }
}
</style>

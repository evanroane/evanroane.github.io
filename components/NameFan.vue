<template>
  <section class="fan">
    <svg
      class="fan-image"
      viewBox="0 0 1350 505"
      xmlns="http://www.w3.org/2000/svg"
    >
      <defs>
        <filter id="inner-glow-red">
          <feFlood flood-color="var(--red)" />
          <feComposite in2="SourceAlpha" operator="out" />
          <feGaussianBlur stdDeviation="3" result="blur" />
          <feComposite in2="SourceGraphic" operator="atop" />
        </filter>
        <filter id="inner-glow-orange">
          <feFlood flood-color="var(--orange)" />
          <feComposite in2="SourceAlpha" operator="out" />
          <feGaussianBlur stdDeviation="3" result="blur" />
          <feComposite operator="atop" in2="SourceGraphic" />
        </filter>
        <filter id="inner-glow-yellow">
          <feFlood flood-color="var(--yellow)" />
          <feComposite in2="SourceAlpha" operator="out" />
          <feGaussianBlur stdDeviation="3" result="blur" />
          <feComposite operator="atop" in2="SourceGraphic" />
        </filter>
        <filter id="inner-glow-yellow">
          <feFlood flood-color="var(--yellow)" />
          <feComposite in2="SourceAlpha" operator="out" />
          <feGaussianBlur stdDeviation="3" result="blur" />
          <feComposite operator="atop" in2="SourceGraphic" />
        </filter>
        <filter id="inner-glow-green">
          <feFlood flood-color="var(--green)" />
          <feComposite in2="SourceAlpha" operator="out" />
          <feGaussianBlur stdDeviation="3" result="blur" />
          <feComposite operator="atop" in2="SourceGraphic" />
        </filter>
        <filter id="inner-glow-blue">
          <feFlood flood-color="var(--blue)" />
          <feComposite in2="SourceAlpha" operator="out" />
          <feGaussianBlur stdDeviation="3" result="blur" />
          <feComposite operator="atop" in2="SourceGraphic" />
        </filter>
      </defs>
      <text
        class="fan-text fan-text--secondary fan-text--secondary__red"
        filter="url(#inner-glow-red)"
        x="200"
        y="500"
      >
        {{name}}
      </text>
      <text
        class="fan-text fan-text--secondary fan-text--secondary__orange"
        filter="url(#inner-glow-orange)"
        x="200"
        y="500"
      >
        {{name}}
      </text>
      <text
        class="fan-text fan-text--secondary fan-text--secondary__yellow"
        filter="url(#inner-glow-yellow)"
        x="200"
        y="500"
      >
        {{name}}
      </text>
      <text
        class="fan-text fan-text--secondary fan-text--secondary__green"
        filter="url(#inner-glow-green)"
        x="200"
        y="500"
      >
        {{name}}
      </text>
      <text
        class="fan-text fan-text--secondary fan-text--secondary__blue"
        filter="url(#inner-glow-blue)"
        x="200"
        y="500"
      >
        {{name}}
      </text>
      <text
        class="fan-text"
        x="200"
        y="500"
      >
        {{name}}
      </text>
    </svg>
  </section>
</template>

<script lang="ts">
export default {
  data() {
    return { name: 'Evan Roane' }
  }
};
</script>

<style scoped>
.fan {
  display: flex;
  cursor: default;
  user-select: none;
  width: 100%;
  justify-content: center;

  --no-opacity: 0;
  --mid-opacity: 0.5;
  --full-opacity: 1;
  --transform-start: rotate(0deg) translate(0%, 0%);
}

.fan-image {
  width: 1000px;
  height: 500px;
}

@media only screen and (min-width: 600px) {
  /* For tablets: */
}

@media only screen and (min-width: 768px) {
  /* For desktop: */
}

.fan-text {
  fill: var(--white);
  font-family: Futura, sans-serif;
  font-size: 200px;
  font-weight: 500;
  transform-box: view-box;
}

.fan-text--secondary {
  fill: var(--black);
  animation-fill-mode: forwards;
  animation-delay: 0.8s;
  animation-duration: 3s;
}

.fan-text--secondary__red {
  animation-name: fanOutRed;
}

@keyframes fanOutRed {
  0% {
    transform: var(--transform-start);
    opacity: var(--no-opacity);
  }
  50% {
    opacity: var(--mid-opacity);
  }
  100% {
    transform: rotate(-20deg) translate(-15%, 7.4%);
    opacity: var(--full-opacity);
  }
}

.fan-text--secondary__orange {
  animation-name: fanOutOrange;
}

@keyframes fanOutOrange {
  0% {
    transform: var(--transform-start);
    opacity: 0;
  }
  50% {
    opacity: var(--mid-opacity);
  }
  100% {
    transform: rotate(-16deg) translate(-12%, 7.1%);
    opacity: var(--full-opacity);
  }
}

.fan-text--secondary__yellow {
  animation-name: fanOutYellow;
}

@keyframes fanOutYellow {
  0% {
    transform: var(--transform-start);
    opacity: 0;
  }
  50% {
    opacity: var(--mid-opacity);
  }
  100% {
    transform: rotate(-12deg) translate(-9%, 6.2%);
    opacity: var(--full-opacity);
  }
}

.fan-text--secondary__green {
  animation-name: fanOutGreen;
}

@keyframes fanOutGreen {
  0% {
    transform: var(--transform-start);
    opacity: 0;
  }
  50% {
    opacity: var(--mid-opacity);
  }
  100% {
    transform: rotate(-8deg) translate(-6%, 4.8%);
    opacity: var(--full-opacity);
  }
}

.fan-text--secondary__blue {
  animation-name: fanOutBlue;
}

@keyframes fanOutBlue {
  0% {
    transform: var(--transform-start);
    opacity: 0;
  }
  50% {
    opacity: var(--mid-opacity);
  }
  100% {
    transform: rotate(-4deg) translate(-3%, 2.7%);
    opacity: var(--full-opacity);
  }
}
</style>

<!--
 * SaaS Makers - Web
 *
 * Copyright 2023, SaaS Makers
 * Author: Valerian Saliou https://valeriansaliou.name/
 -->

<!-- **********************************************************************
     TEMPLATE
     ********************************************************************** -->

<template lang="pug">
.c-page-wrapper
  slot
</template>

<!-- **********************************************************************
     STYLE
     ********************************************************************** -->

<style lang="scss">
$c: ".c-page-wrapper";

// VARIABLES
#{$c} {
  width: calc(100% - (2 * $page-wrapper-default-padding-sides));

  max-width: calc(
    $page-wrapper-max-width - (2 * $page-wrapper-default-padding-sides)
  );

  margin: 0 auto;
  padding: 0 $page-wrapper-default-padding-sides;
}

// --> MEDIA-QUERIES <--

@media (max-width: $screen-large-width-breakpoint) {
  #{$c} {
    max-width: auto;
  }
}

@media (max-width: $screen-medium-width-breakpoint) {
  #{$c} {
    width: calc(100% - (2 * $page-wrapper-medium-padding-sides));
    padding: 0 $page-wrapper-medium-padding-sides;
  }
}

@media (max-width: $screen-small-width-breakpoint) {
  #{$c} {
    width: calc(100% - (2 * $page-wrapper-small-padding-sides));
    padding: 0 $page-wrapper-small-padding-sides;
  }
}

@media (max-width: $screen-tiny-width-breakpoint) {
  #{$c} {
    width: calc(100% - (2 * $page-wrapper-tiny-padding-sides));
    padding: 0 $page-wrapper-tiny-padding-sides;
  }
}

@media (max-width: $screen-lilliput-width-breakpoint) {
  #{$c} {
    width: calc(100% - (2 * $page-wrapper-lilliput-padding-sides));
    padding: 0 $page-wrapper-lilliput-padding-sides;
  }
}
</style>

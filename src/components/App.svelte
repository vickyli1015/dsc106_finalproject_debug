<script>
  import ScrollyTeller from '../components/ScrollyTeller.svelte';

  // Your slides array, containing paths to images or SVG content
  const slides = [
    'first_page.svg',
    'no_talking.svg',
    'defect-silent.svg',
    'silent-defect.svg',
    'defect-defect.svg',
    'silent-silent.svg',

    'matrix_start.svg',
    'matrix_silent.svg',
    'matrix_mix.svg',
    'matrix_defect.svg',
    'interact_given_cooperate.svg',
    'outcome_given_cooperate.svg',
    'interact_given_defect.svg',
    'outcome_given_defect.svg',
  ];
</script>

<ScrollyTeller {slides} />

<style>
  /* Additional styling as needed */
</style>
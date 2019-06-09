<template lang="html">
  <div>
    <main>
      <h2>About Merlin Movie House</h2>
      <div class="flex-container">
        <div>
          <img src="https://lh3.googleusercontent.com/CjgRdedtdD6Vfc83CKuQDKSanUpY0u3t-UlkdrJvHQPcVUH1LZa6-9XyyI7zntufli52_gGngmFzFDxaId8--cMVBU37DGVNrraC-yQvUVbPlg1aYE2ceIkXnRS3ugEZKinbT-UeZmN7KiAiMzGkYVrvPmx943f15Ii4sDuz7PUKAPZEX63f41iFvuzTqdzqOJge-ehkfIlnqoDlGwwxO_FWdzYeGIQB7Pp_XyaP2sxclOOE3T-vmmrQmUqqFCvepYUSlyM4OSwClNAhgEPzsHxKp8slUAYBa8RIpmRD8g4Aiaw6xdiZWzU_HiwmgJHMEPa99Afy47neTrLs_jw1joC36ooeDGhZQLNPF3TRHguV90r5dmVyG-81nydH6U_YUYKhv0b25iip6P1ZbN8dYJpMYoA9_tDjQqs7Qh9rZYtDjAyX0JYWaOxygYKFJgUgb-GTcVXgXkTzYG7W9egeXRGBUy2cO5aKsfqzd1vJ1aGHLUl7nErV3HNmjOV7KgbGUpOaQKbOPAzYYJDXnyxB79Ll0Hd_DpWQzmrmo2XHwri-ZrWc5Qqp6E2SuBne_fCTX3FgEUmrbtUA4t19mwwzmMc2jqxf-LTy7MqPY9pbpSTprANc1qnxDfANZzW_zOADVXcCyirjGFKkct6yAkqgX_d95QboHvQ=w960-h520-no" alt="Screen One" class="img-thumbnail">
        </div>
        <div>
          <img src="https://lh3.googleusercontent.com/zuVB_P5i0xDQqH6aIAZj7mczOFE989daSr9BBb828w0Rgcer--GZhqpyT1dStaUIMARjeSPDOTo4aA7QJ1cvqi-AZAWCfZ5gONEns28IEHiPTVO_NHhGCwQ42yF05UE6rJEml63-1uMPHgYx2cXrWDCUUnSeZmeun_J2sOaQzPqFFouqOgiSS8D5FePL0F3EhzVi4afp7lm2-GSX4MZZn7TU5ieK5stQmJtgBHhixumyfpFh0bgQ2tLVVUbAt0o5Yro2fkKCZ4T4hY0poCdDcqoZ5qx8fbiM7Jg7hCSAOPWpbAjBrM2DVSoBwQf5dHvCPjMqOU6cWAcqQildpy4pUQhr14ywkrVbuVSJOGRfEznVVLULHxP3TN0Jvr4ow__EBUhexR9E9JvvLv2j6YA-OvpKuhCpPXwuG4rkVU8iC3yZw5eM3ab5vKnb_N6kXRWLB5avTJC9OOD6wYcOhUZF7YOFGaquUyFvian2Dko5lm6Z9q30qawGJyVvJeuGioUDxboKfu3_l5fwrRLQCicEnzCeqizEQ28GOwoWOj5fwAF_MycGi6Yo6ZoMtRTbcdJOewbr4B6qFyy7JE6yRLjD1qJn-eKfT0Ra2stvHTy6tqDVkZwsgMDhvCkZqD9pxWEjF3a7cXxdt-jK2GhjkJxYkuI0YThjRfQ=w960-h520-no" alt="bar" class="img-thumbnail">
        </div>
      </div>
      <article>
        <p>The Merlin Movie House was opened in Seattle's Beacon Hill neighborhood in 2015.
           The two screen cinema is housed in a historic theater, which was completely
           refurbished when the Merlin's acquired it in 2014.</p>
        <h4>The Screens</h4>
        <p>Screen one is the largest auditorium and can seat up to 500 people. It maintains the
        original theater aesthetic and has kept many of its decorative flourishes.</p>
        <p>Screen two is a more modern and intimiate space. It boasts 4K projection,
        Dolby Surround Sound, and reclining seats for a potential 100 guests.</p>
        <h4>The Bar</h4>
        <p>The bar area can hold up to 200 people and features a 30 foot long
        original wooden bar. Rotating taps feature the best of the local craft beer scene,
        and our bar snacks are all locally made and sourced.</p>
      </article>
    </main>
  </div>
</template>

<script>
export default {
}
</script>

<style scoped>
nav {
  font-family: Merriweather;
}
main {
  margin: 2rem 3rem;
  font-family: Merriweather;
}
.flex-container {
  display: flex;
  flex-wrap: wrap;
  flex-direction: row;
  overflow: hidden;
  /* width: 100%; */
}

.flex-container div {
  padding: 0.5rem;
  width: 48%;
  font-size: 0.75rem;
  min-width: 200px;
}

.img-thumbnail {
  margin: 0;
}

</style>

<template lang="html">
  <div>
    <main>
      <h2>Gallery</h2>
      <p>See photos of our space and some of the events we've held.</p>
      <AppGallery v-bind:images="images"></AppGallery>
  </main>
  </div>
</template>

<script>
import AppGallery from '../components/AppGallery.vue';

export default {
  components: {
    AppGallery,
  },
  data () {
    return {
      images: [ {src: 'https://lh3.googleusercontent.com/AUzW6bHCkEzlgAP15_NFRgHuL5iBkW8Uo_2enhEC9GxxH4dWJlt7eGIJqNa3apafI9K2QMvVlYc_q4BjZKnQvrNMGKNce7zi5grsZFEeMPBFO-vkycswJzL3XO09QAYnzUs_nNe6x0jc6MGApvD8NJdrqJs_p0UHpNxYP62eN6kvNmMlvTRjWxG6hECtM10-U84tWqn491OkmvbctL-z4om2X7_9vZH4R-XLQkfh7ZvE9f4uLXndLB2v79PaOEIYRvoP-9Yw4xKEzDK6aDGtOtaIvKlt3klAM5ICG_mstBysgTvu0TpJGoicbDo9BLCNh8RrcPE_rJ-ce6X920dHGzWtO2wFMhHUkt0xLNtiJgtPXaWDMgSKwe-kxmK3i5dvHn4449cnvoIdaqGy0eQnbrlcwIy7yeYAOuAaXDlx3DUlWYEVcXVwO5t0dKuHaciKcWxzGen7DM5SCNRSPG9XPdMV0QmN6P4QQmWfE2Y2Unukiy5GZg9xuoC5e-kK5iPCLVJC3BVoEU64zmuVR0OpTIWohDs2U-Ud8XipS65wbCNIUGlMlqWEgEozn1V3mFxxoyXGg5Y_JO7ENWN9uElkqbVDBE_8T5Lz2IaXptrCwWrFXwl-Dpe6mwt_oYdoB4uHzZwRVUa_bXfSir87_xdcWK6Errz1BQk=w960-h520-no', alt: 'snacks', title: 'Tasty Film Snacks', description: 'Vegan and gluten free options available at our bar.' },
                {src: 'https://lh3.googleusercontent.com/CjgRdedtdD6Vfc83CKuQDKSanUpY0u3t-UlkdrJvHQPcVUH1LZa6-9XyyI7zntufli52_gGngmFzFDxaId8--cMVBU37DGVNrraC-yQvUVbPlg1aYE2ceIkXnRS3ugEZKinbT-UeZmN7KiAiMzGkYVrvPmx943f15Ii4sDuz7PUKAPZEX63f41iFvuzTqdzqOJge-ehkfIlnqoDlGwwxO_FWdzYeGIQB7Pp_XyaP2sxclOOE3T-vmmrQmUqqFCvepYUSlyM4OSwClNAhgEPzsHxKp8slUAYBa8RIpmRD8g4Aiaw6xdiZWzU_HiwmgJHMEPa99Afy47neTrLs_jw1joC36ooeDGhZQLNPF3TRHguV90r5dmVyG-81nydH6U_YUYKhv0b25iip6P1ZbN8dYJpMYoA9_tDjQqs7Qh9rZYtDjAyX0JYWaOxygYKFJgUgb-GTcVXgXkTzYG7W9egeXRGBUy2cO5aKsfqzd1vJ1aGHLUl7nErV3HNmjOV7KgbGUpOaQKbOPAzYYJDXnyxB79Ll0Hd_DpWQzmrmo2XHwri-ZrWc5Qqp6E2SuBne_fCTX3FgEUmrbtUA4t19mwwzmMc2jqxf-LTy7MqPY9pbpSTprANc1qnxDfANZzW_zOADVXcCyirjGFKkct6yAkqgX_d95QboHvQ=w960-h520-no', alt: 'auditorium', title: 'Screen One', description: 'Our largest auditorium seats up to 500.'},
                {src: 'https://lh3.googleusercontent.com/S11o0OI9bCb2603Kjh0mUP0-ASp6U8N6rOpdw69SXKp4wHRvgR_m9OKq0ah1ruASu6t8GLjzqRW_ve2R7Yjhmpwj9UyIlyIO4car0wpr61QAtxyGImyIzZmpSqmYLOcPl7afDwkv8iV8fZLQ25AYS5CCc6-Ktgwmmj2ldGFD3W5s8FYA8zhibOX-bsPMQYdqNW_hibHDFzIhVbIfeggpE9uEFJUbPn_D_7PaNcOEAgj399ZiR9gByvfVXHoFrtuwlcFEI_lyzn6ZtcX0ZMb22WPPxj5Tv01NMSpVhJvP2sM-dsRdRbSPPUYwrtAMwYYyNZ8jwwQCuFiEKYRuPA3TwMHpKSNYSM6ZsNgkGn0_l9z9D3vZg7eHp5l3Il9H1jyoYsM_MDVqD2lHOP5o-wPz3qXBuXkbYn6ROJQNe_J-UNGAgVYA6sxHUmr-_EE8eP_O6bhe2XXLyVxkTHYgap_MswT-qu68axWegF1wXxRpCcciBIkLEB9PgFKfccP0Dg1eTcBd7AJgt1oBV0E-BRzxmfkqfP29ivnM3X2A4N0w-2Nd9ZdUsgPLB1XfgoLNO_hNsGIHnPQbCAdtpLM4HD1Ua1xnGkuNxVbN-76Pbe27zgbH2RHzILwG4CqCSzIDUp-LFCRsP8Ag4jPvHGVb3YmX6LMAPQV33U8=w960-h520-no', alt: 'craft beer', title: 'Local Craft Beer', description: 'Try a pint from one of the neighborhood craft breweries.'},
                {src: 'https://lh3.googleusercontent.com/zuVB_P5i0xDQqH6aIAZj7mczOFE989daSr9BBb828w0Rgcer--GZhqpyT1dStaUIMARjeSPDOTo4aA7QJ1cvqi-AZAWCfZ5gONEns28IEHiPTVO_NHhGCwQ42yF05UE6rJEml63-1uMPHgYx2cXrWDCUUnSeZmeun_J2sOaQzPqFFouqOgiSS8D5FePL0F3EhzVi4afp7lm2-GSX4MZZn7TU5ieK5stQmJtgBHhixumyfpFh0bgQ2tLVVUbAt0o5Yro2fkKCZ4T4hY0poCdDcqoZ5qx8fbiM7Jg7hCSAOPWpbAjBrM2DVSoBwQf5dHvCPjMqOU6cWAcqQildpy4pUQhr14ywkrVbuVSJOGRfEznVVLULHxP3TN0Jvr4ow__EBUhexR9E9JvvLv2j6YA-OvpKuhCpPXwuG4rkVU8iC3yZw5eM3ab5vKnb_N6kXRWLB5avTJC9OOD6wYcOhUZF7YOFGaquUyFvian2Dko5lm6Z9q30qawGJyVvJeuGioUDxboKfu3_l5fwrRLQCicEnzCeqizEQ28GOwoWOj5fwAF_MycGi6Yo6ZoMtRTbcdJOewbr4B6qFyy7JE6yRLjD1qJn-eKfT0Ra2stvHTy6tqDVkZwsgMDhvCkZqD9pxWEjF3a7cXxdt-jK2GhjkJxYkuI0YThjRfQ=w960-h520-no', alt: 'the bar', title: 'Our Cinema Bar', description: 'Our beautiful bar is the perfect spot for a pre-movie tipple.'},
                {src: 'https://lh3.googleusercontent.com/yjGsqb2uZDvJKUteycJG0K-ZaGXHPPsjIvd15XSaGEn17nOdMoSk7qw65Zd4Jd5iKF9_EqLw_QTuCNPymnWV0qYsN-7rDp32n6jeMFZleA2s35jrAf73ODOthfORtgirBtu0cjY_sR2uTX6Go8HJ8o8l2SUyoXgfFrnFsCZ1d7bbNnGcNXPK7qWgaxZ8XsOn4edFyjPGX8OEC36PER-QP7m7JF0bIjkyZirDFQc9QzAaTstJ8k0mlD8l7dMvH7-GNG60GTsKrsUjWYe-QlPLTwI_IgNv-ZO-U1E-CLc0fm07LF4mFJNLfZ75lLv2l64xRWF2KhnSHAdkSiLIrBo6QQXLC62y15o8JHbF13ljDSkS8dIUxaZ4VwUXBRLo9OamdXvKRw47WxwbuRhNKhNQwCCve6ZjWJZDvfWxKEGWeeEv6NqQI-MObbBgiUnOylxow8WUqPDqLc9Q6qz60UJi16qK6wZvw3QWlniTdcc8u3sMEWZsS7VV31_Tp44S-G98wdst80O8TEi-BXn7jN5PbJNQUsbE1foRUj-JGjhOxzQldLzoaTZdnYr_ETOADxzbQcM-PSkwup8Wox6hLafG_oh1sfEsZcFO2UJvFnKYWTbM_cOx658BdA6tm08BsDkamku17q3s__fzWkjBpSg1xdpFQDV4SqI=w960-h520-no', alt: 'audience', title: 'Beacon Hill Film Fest', description: 'Supporting the film community by hosting film festival screenings. '},
                {src: 'https://lh3.googleusercontent.com/uTbd5L2E86x68WVIBNyJVMtLkyo6iYgQXVlEZwFty2E16OMEiNrI4xKQnf1aHVo-2V6-ndXtnGWyT0OBXc7Zqg0VYeEEMbviwU8ENBQniJlc3GXqzgRHjMMbdy6YR_7vnXeDj4nmDFUAv39aXy-OaHNcGQENA8j4E32XBumLwGfYqvlhZx30aBzD5EYtfFUr0oz9ZGcraeupAQOdjjarw8DH4c6jGdMgKjScYkBMlmVQu84vWVCpkP908rTI_oDL4mkUuTQWkXYyEeEmAIGY2Pux1-Q4VjyAjy0f3Kvm_sdVJn43sYOWgYFsvmCdmwldvX6nvNztSEBEjY4zBVmdXKvYoxvgYS0zxrW7jx9kX1mc1KcsepEKHaX29IeqU4buNkHeh3tbE8E10FWvb179vwQPaKrMc0Emk--IAK4ggZE_iytWgeSfDlQLk78Ld4P6YBn0qqcyWloZbM7-rAXWhgW3LhD4WZ-LXsx3rTZnNP26oqBZH8-Suh202Rfh0zQMyd3H_RkPqokqQ7hRGzlG6uTp2HezoyZsalKIkVmMOyZZSjU9Xcv2lf0rZKUHQEjLdCp6kqW1B4F2LXHa9OljN1C7kO6NZqM6CXOXOf17l1mt_66bNKv0x6LurWkaO0dHWR462lGM1bhHCdhrPTzYBZhDhNu77g0=w960-h520-no', alt: 'auditorium 2', title: 'Screen Two', description: 'Our second screen seats up to 100.'}
            ]
    }
  }
}
</script>

<style lang="css" scoped>
main {
  margin: 2rem 3rem;
  font-family: Merriweather;
}
</style>

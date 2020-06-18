<template>
  <f7-page name="Details">
    <f7-navbar title="Details"></f7-navbar>
    <f7-card>
      <f7-card-content>
        <div v-html="content"></div>
      </f7-card-content>
    </f7-card>
  </f7-page>
</template>

<script>

  const SIMULATED_CONTENT = "<p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Curabitur luctus rutrum diam, non tincidunt metus rhoncus non. Duis euismod ultrices convallis. Donec leo ipsum, accumsan eget condimentum et, porttitor eu purus. Ut eleifend tempor mattis. Proin eu odio mauris. Duis a suscipit est. Mauris in lectus et neque molestie scelerisque. Maecenas finibus congue neque, vitae tristique metus fringilla quis.</p>" +
    "<p>Cras mattis turpis enim, vel vulputate turpis pulvinar sit amet. Nulla molestie sapien at rutrum imperdiet. Etiam sit amet massa a nisl pharetra imperdiet. Mauris fringilla hendrerit dui, ut hendrerit ligula mattis non. Nullam a interdum augue, ac venenatis mauris. Mauris sit amet ipsum a ipsum aliquet ullamcorper. Aenean bibendum lacus arcu, a semper leo efficitur at. Nulla facilisi. Donec non consequat lorem. Donec volutpat erat et nisi imperdiet, ac pretium neque pharetra. Suspendisse vitae rutrum mi. Etiam eu aliquet purus. Nam ut metus sed erat ultricies lobortis consectetur eu ipsum.</p>" +
    "<p>Nullam eleifend placerat metus. Duis eleifend augue eu tincidunt malesuada. In nec ultricies diam, sed ornare eros. Nulla facilisi. Nullam condimentum sagittis ex in rutrum. Pellentesque id metus a justo semper imperdiet. Morbi sit amet mollis libero. Vestibulum quis interdum libero. Suspendisse venenatis magna eu turpis tempor consectetur. Aliquam turpis arcu, iaculis hendrerit sapien ut, eleifend euismod sem. Phasellus sodales, mi et sollicitudin posuere, augue lectus condimentum metus, et vestibulum nibh sapien eget ante. Morbi sodales, velit at pharetra congue, ante orci pretium orci, quis tempus massa dui nec ex. Nullam dapibus eros nec leo suscipit, ut facilisis quam pellentesque. Curabitur ac eros turpis. Proin dignissim at sapien sit amet pretium</p>" +
    "<p>Sed id fermentum sem. Aliquam sed quam ac turpis blandit aliquam id at nibh. Vivamus lorem erat, tincidunt a mollis at, rutrum vel felis. Sed ut sem tristique, tempus purus ut, interdum enim. Vestibulum at commodo ipsum, vel suscipit tortor. Pellentesque accumsan elit quis arcu fermentum, sed cursus nulla molestie. Fusce eu diam in elit mollis hendrerit. In eu felis eget nisl suscipit aliquet. Nunc risus nisl, molestie a laoreet in, feugiat at lorem. Nam efficitur accumsan tortor, eget imperdiet ipsum maximus sed. Quisque porttitor fringilla sodales. Fusce at dapibus ex, eu facilisis massa. In efficitur feugiat convallis. Integer sapien dolor, auctor in odio finibus, tristique laoreet massa. Curabitur quis urna ac enim feugiat eleifend.</p>" +
    "<p>Vestibulum at massa felis. In urna erat, ornare vitae quam non, ultrices semper erat. Vestibulum porttitor lacus dolor, non sodales est rhoncus a. Duis ut mattis nibh. Integer tempus id libero id posuere. Maecenas id dui urna. Ut dictum dapibus quam nec feugiat. Vivamus accumsan porta interdum. In auctor magna in maximus vulputate. Nam quis dui imperdiet risus feugiat tincidunt. Vestibulum ante ipsum primis in faucibus orci luctus et ultrices posuere cubilia curae; Donec suscipit augue at nunc bibendum accumsan. Fusce faucibus, ante at lacinia commodo, massa elit ultricies massa, non pellentesque elit augue in justo.</p>"

  export default {
    data: function() {
      return {
        content: ''
      }
    },
    created: function() {
      setTimeout(() => {
        // simulating API call
        this.content = SIMULATED_CONTENT
      }, 100)
    }
  }
</script>

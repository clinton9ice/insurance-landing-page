<template>
  <div class="bg-success-20 slant py-4 my-5">
    <br />
    <br />
    <Section class="mt-5 py-4">
      <div class="row align-items-end justify-content-between">
        <div class="col-lg-5 col-md-8 col-sm-8 px-3">
          <h4 class="tag text-success mt-lg-5 small">100% claims assessment</h4>
          <br />

          <h1 class="display-5 fw-bold text-navy" data-aos="fade-in" data-aos-delay="300">Make claims with ease</h1>
          <br />
          <p class="text-muted fw-bold" data-aos="fade-up" data-aos-delay="500">
            Our digital self-inspection process lets your team report issues in
            real-time keep your business running non-stop.
          </p>
          <br />
          <br />
          <ul class="list-container">
            <li class="list-item selected">
              <div class="ps-3">
                <h6 class="fw-bold">Report claim</h6>
                <p class="des small text-muted">
                  It all starts with a quick click. Login in to your bank from
                  any device.
                </p>
              </div>
            </li>

            <li class="list-item">
              <div class="ps-3">
                <h6 class="text-muted">Take Picture</h6>
              </div>
            </li>
            <li class="list-item">
              <div class="ps-3">
                <h6 class="text-muted">Estimate damage</h6>
              </div>
            </li>
            <li class="list-item">
              <div class="ps-3">
                <h6 class="text-muted">Get paid</h6>
              </div>
            </li>
          </ul>
        </div>

        <div class="col-lg-4 col-md-8 col-sm-10 overflow-hidden my-5">
          <div class="img-thumbnail-circle">
            <img
              src="../static/img/icons/phone.png"
              class="w-100"
              alt="assessment"
              data-aos="fade-up" data-aos-delay="300"
            />
          </div>
        </div>
      </div>
    </Section>
  </div>
</template>

<script>
import Section from "./Section.vue";
export default {
  components: { Section },
};
</script>

<style scoped>
.img-thumbnail-circle {
  height: 400px;
  width: 400px;
  border-radius: 50%;
  background-color: var(--success-50);
  overflow: hidden;
}
.list-container .list-item {
  padding: 0.1rem 0.4rem;
  border-left: 3px dashed var(--bs-gray-300);
  list-style: none;
  margin-bottom: 1rem;
}
.list-container .list-item.selected {
  border-left-style: solid !important;
  border-color: var(--bs-indigo);
}
.list-container .list-item:not(.selected) {
  padding: 1.5rem 0.5rem;
}
.slant {
  position: relative;
  overflow: hidden;
}
.slant::before {
  content: "";
  position: absolute;
  top: -90px;
  height: 203px;
  width: 100vw;
  background-color: var(--bs-white);
  transform: rotateZ(7deg);
  border-bottom: 3px solid var(--success-50);
  box-sizing: border-box;
}
</style>

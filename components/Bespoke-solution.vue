<template>
  <Section class="mt-5 py-4">
    <div class="row align-items-end justify-content-between">
      <div class="col-lg-5 col-md-8 col-sm-8 px-3">
        <h4 class="tag text-success mt-lg-5 small">Bespoke solutions</h4>
        <br/>

        <h1 class="display-5 fw-bold text-navy">
          One-in-all Solution for Business
        </h1>
        <br/>
        <p class="text-muted fw-bold" data-aos="zoom-in" data-aos-delay="300">
          We empower you with data via a web interface for managing plans and
          staff to drive better management decisions
        </p>
        <br/>
        <br/>
        <ul class="list-group">
          <li class="list-item purple active"><span>Plans</span></li>
          <li class="list-item orange"><span>Claims</span></li>
          <li class="list-item success"><span>Beneficiaries</span></li>
          <li class="list-item success"><span>Wallet</span></li>
        </ul>
      </div>

      <div class="col-lg-6 col-md-8 col-sm-10 overflow-hidden my-5" data-aos="fade-up" data-aos-delay="400">
        <img
          src="../static/img/Frame-94092.jpg"
          class="w-100 ms-5 ps-5"
          alt="Empowerment"
        />
      </div>
    </div>
  </Section>
</template>

<script>
export default {};
</script>

<style scoped>
.list-group .list-item {
  padding: 1.2rem 1rem;
  background: #fff;
  box-shadow: 0 6px 12px #0000000d;
  margin-bottom: 1rem;
  border-radius: 4px;
  border-left: 4px solid;
  opacity: 0.7;
  transition: all 400ms ease;
  cursor: pointer;
}
.list-group .list-item.purple{
  border-color: #7A5AF8;
}
.list-group .list-item.orange{
  border-color: #FCCEEE;
}
.list-group .list-item.success{
  border-color: var(--success-50);
}
.list-group .list-item.purple{}

.list-group .list-item:hover, .list-group .list-item.active{
  opacity: 1;
  box-shadow: 0 10px 12px #0000000d;
}

@media screen and (max-width: 650px){
  .list-group{
    display: flex;
    overflow: hidden;
    overflow-x: auto;
    width: 100%;
    flex-direction: row;
    justify-content: space-between;
  }
  .list-group::--webkit-scrollbar{
    height: 2px;
  }
  .list-group .list-item{
    width: 50%;
    flex-shrink: 0;
  }
}
</style>

<template>
<link rel="stylesheet" href="">
  <div class="card">
    <div class="card1">
      <div class="img">
        <img src="../img/doctors-1.jpeg" alt="" />
      </div>
      <div class="info">
        <h4>Bath Dorgeles</h4>
        <span>Cohorte 5</span>
        <p>+225 0143396552</p>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "CardAnnuaire",
};
</script>

<style lang="scss">
.card {
  width: 30%;
  padding: 20px;
  &:hover {
    .img {
      img {
        scale: 1.2;
      }
    }
  }
  .card1 {
    display: flex;
    justify-content: space-between;
    background: #fff;
    position: relative;
    box-shadow: 0px 2px 15px rgb(44 73 100 / 8%);
    padding: 30px;
    border-radius: 10px;
    padding-right: 20%;

    .img {
      overflow: hidden;
      width: 180px;
      border-radius: 50%;
      background: #fff;
      img {
        transition: ease-in-out 0.3;
        max-width: 100%;
        height: auto;
      }
    }

    .info {
      position: relative;
      top: 20px;
      right: 20px;

      h4 {
        font-weight: 700;
        margin-bottom: 5px;
        font-size: 20px;
        color: #f16e00;
      }

      span {
        display: block;
        font-size: 15px;
        padding-bottom: 10px;
        position: relative;
        font-weight: 500;
        color: #111;
        right: 30px;
        &::after {
          content: "";
          position: absolute;
          display: block;
          width: 50px;
          height: 1px;
          background: #f16e00;
          bottom: 0;
          left: 30px;
          padding-left: 20px;
        }
      }
    }
  }
}
</style>

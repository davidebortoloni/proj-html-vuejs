<template>
  <div id="calls-to-action">
    <div class="container-fluid">
      <div class="row">
        <div class="col-6">
          <div id="new-project" class="w-100 call">
            <div class="question mb-3">Are you ready?</div>
            <h3 class="mb-5">Start a New Project</h3>
            <div class="form">
              <input type="email" placeholder="Enter Your Email Address" />
              <button>SUBMIT</button>
            </div>
          </div>
        </div>
        <div class="col-6">
          <div id="lets-talk" class="w-100 call">
            <div class="question mb-3">What Are You Waiting for?</div>
            <h3 class="mb-5">Let's Talk About Work</h3>
            <button class="button btn-reverse">Start Now</button>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "CallsToAction",
};
</script>

<style scoped lang="scss">
@import "../../assets/scss/_vars.scss";

#calls-to-action {
  margin-bottom: 100px;
  #new-project {
    background: linear-gradient(90deg, $thirdColor, $fourthColor);
  }
  #lets-talk {
    background: linear-gradient(90deg, $mainColor, $secondaryColor);
  }
  .call {
    color: white;
    border-radius: 10px;
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    height: 350px;
    .question {
      font-family: "Quicksand", sans-serif;
      font-size: 18px;
      font-weight: 600;
    }
    .form {
      width: 65%;
      padding: 20px;
      border-radius: 30px;
      background-color: #3f3f3f;
      font-family: "Quicksand", sans-serif;
      font-size: 18px;
      font-weight: 600;
      input {
        width: 80%;
        background-color: transparent;
        border: none;
        &:focus {
          outline-width: 0;
        }
      }
      button {
        background-color: transparent;
        border: none;
        width: 20%;
        color: $sixthColor;
        font-family: "Quicksand", sans-serif;
        font-size: 15px;
        font-weight: 600;
      }
    }
  }
}
</style>
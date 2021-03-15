<template>
  <div>
      <div id="banner">
          <b-container>
            <b-row class="justify-content-md-center  no-gutters">
                <b-col cols="12" lg="6">
                    <h1 class="banner-text pb-5">Australia's most trusted trades provider</h1>
                    <b-form @submit="onSubmit" @reset="onReset" v-if="show">
                    <b-form-group id="input-group-1" label="What trade do you need?" class="form-input pb-4" label-for="input-1">
                      <font-awesome-icon icon="tag" />
                        <b-form-input
                        id="input-1"
                        v-model="form.trade"
                        type="text"
                        placeholder="e.g Plumber, Electricians"
                        required
                        ></b-form-input>
                    </b-form-group>

                    <b-form-group id="input-group-2" label="Postcode or Suburb:" class="form-input" label-for="input-2">
                      <font-awesome-icon icon="map-marker-alt" />
                        <b-form-input
                        id="input-2"
                        v-model="form.postcode"
                        placeholder="e.g Sydney"
                        required
                        ></b-form-input>
                    </b-form-group>
                    <b-row class="justify-content-md-center mt-5">
                      <b-col cols="12" md="8"> <b-button type="submit" variant="danger btn-block glow shadow btn-submit">Post a Job</b-button></b-col>
                    </b-row>
                   
                    </b-form>
                </b-col>
            </b-row>
        </b-container>
      </div>
  </div>
</template>

<script>
  export default {
    data() {
      return {
        form: {
          trade: '',
          postcode: ''
        },
      
        show: true
      }
    },
    methods: {
      onSubmit(event) {
        event.preventDefault()
        alert(JSON.stringify(this.form))
      },
      onReset(event) {
        event.preventDefault()
        // Reset our form values
        this.form.email = ''
        this.form.name = ''
        this.form.food = null
        this.form.checked = []
        // Trick to reset/clear native browser form validation state
        this.show = false
        this.$nextTick(() => {
          this.show = true
        })
      }
    }
  }
</script>

<style lang="scss">
$primary-color:#475f7b;
$secondary-color:#2c3e50;
$third-color:#727e8c;
$lavender-color:#7367f0;


$font-stack:    Helvetica, sans-serif;

@mixin box-shadow($property) {
  -webkit-box-shadow: $property;
  -ms-box-shadow: $property;
  box-shadow: $property;
}

#banner{
    padding: 80px 0;
}

h1.banner-text{
    font-size: 65px;
    font-weight: 600;
    text-align: center!important;
    margin-bottom: 1rem!important;
    color:$primary-color;

    @media only screen and (max-width: 767px) {
      font-size: 50px;
    }
    @media only screen and (max-width: 425px) {
      font-size: 40px;
    }
}

form {
    label{
        font-size: 18px;
        color:$primary-color;
        font-weight: 800;
        text-align:left;
    }
    input{
        padding: 30px 50px !important;
    }
    
}

.form{
    &-input > div {
      position: relative;
    }
    &-input > div svg {
      color: #828D99;
      position: absolute;
      top: 25px;
      left: 20px;
    }
}

.shadow{
    @include box-shadow(0 2px 4px 0 rgba(255,91,92,.5));
}
.btn-submit {
    padding: 17px !important;
    color: #fff;
    background-color: #FF5B5C !important;
    border-color: #FF5B5C !important;
}
.btn-danger{
    // border-color: #ff2829!important;
    background-color: #ff5b5c!important;
    color: #fff;
  &:hover{
    &.glow {
      -webkit-box-shadow: 0 4px 12px 0 rgba(255,91,92,.6)!important;
      box-shadow: 0 4px 12px 0 rgba(255,91,92,.6)!important;
    }
  }
}


</style>
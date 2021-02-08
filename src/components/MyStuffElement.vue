<template>
    <b-list-group-item class="rootItem">
        <b-container>
            <b-row>
                <b-col class="col-sm" id="col" sm="12" md="4">
                    <img src="require(this.img)" alt="Item Img" id="itemImg">
                </b-col>
                <b-col class="col-sm" id="col" sm="12" md="4">
                    <h2>{{name}}</h2>
                    <p>{{desc}}</p>
                </b-col>
                <b-col class="col-sm" id="col" sm="12" md="6">
                    <a href={link}>Get it here</a>
                </b-col>
            </b-row>
        </b-container>
    </b-list-group-item>
</template>

<script>
// @ is an alias to /src

export default {
  name: "MyStuffElement",
  props:{
      img: String,
      name: String,
      desc: String,
      link: String
  }
};
</script>

<style>
.rootItem{
    width: 100%;
    height: 100%;
    margin-bottom: 1em;
}
#itemImg{
    margin: auto;
    display: block;
    width: 200px;
}
</style>

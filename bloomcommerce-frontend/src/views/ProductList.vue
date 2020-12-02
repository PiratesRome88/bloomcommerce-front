<template>
  <div class="product-list">
      <h1>Product List</h1>
      <b-card-group deck>
          <b-card v-for="product in products" :key="product.id" title="Card Title"
              img-src="https://picsum.photos/600/300/?image=25" img-alt="Image" img-top tag="article"
              style="max-width: 20rem;" class="mb-2">
              <b-card-text>
                  {{ product.title }}
              </b-card-text>
              <b-card-text>
                  {{ product.description }}
              </b-card-text>

              <b-button :to="{path: '/product/' + product.id}" variant="primary">Buy</b-button>
          </b-card>
      </b-card-group>
      </div>
</template>

<script>
import {
    BCard,
    BCardGroup,
    BCardText,
    BButton
} from 'bootstrap-vue'

export default {
    name: "ProductList",
    components: {
        BCard,
        BCardGroup,
        BCardText,
        BButton
    },
    data(){
        return { 
            products: [
                {   
                    id: '123904',
                    title: 'cat',
                    description: 'my cat'
                },
                {   
                    id: '234456',
                    title: 'dog',
                    description: 'my dog'
                },
                {   
                    id: '876434',
                    title: 'rabbit',
                    description: 'my rabbit'
                },
                                {   
                    id: '234234',
                    title: 'cat',
                    description: 'my cat'
                },
                {   
                    id: '454545',
                    title: 'dog',
                    description: 'my dog'
                },
                {   
                    id: '565656',
                    title: 'rabbit',
                    description: 'my rabbit'
                }
            ]
         };
    },
};
</script>
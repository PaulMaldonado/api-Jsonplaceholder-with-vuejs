<template>
    <div>
        <div class="container">
            <div class="row">
                <div class="col s4">
                    <Card 
                    v-bind:title="album.title"
                    v-for="album in albums" 
                    :key="album.id" />
                </div>
            </div>
        </div>
    </div>
</template>

<script>
import axios from 'axios';
import env from '../config/env';
import Card from '../components/Card';

export default {
    components: {
        Card
    },
    data() {
        return {
            albums: [],
        }
    },

    created() {
        axios.get(`${env.endPoint}/albums`)
            .then(response => {
                this.albums = response.data;
                console.log(response);
            }) 
            .catch(error => {
                console.log(error);
            });
    }
}
</script>

<style scoped>
    
</style>
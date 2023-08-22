<script>
import axios from 'axios';

export default {
    name: 'headerApp',
    mounted() {
        axios.get('http://localhost:8000/api/v1/project-api').then(response => {
            const data = response.data;
            console.log(data);
        }).catch(error => {
            console.log(error);
        });
    }
}
</script>

<template>
    <h1>
        hello world
    </h1>
</template>
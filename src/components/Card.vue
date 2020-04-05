<template>
    <div>
        <div class="container">
            <div class="row">
                <div class="col s4 m12">
                    <div class="card">
                        <div class="card-content">
                            <span class="card-title">{{ title }}</span>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    name: 'Card',
    props: [
        'title'
    ]
}
</script>

<style scoped>
    
</style>
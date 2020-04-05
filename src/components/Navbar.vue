<template>
    <div>
        <div class="navbar-fixed">
           <nav>
               <div class="nav-wrapper">
                   <a href="" class="brand-logo">{{ navTitle }}</a>
                   <ul class="right hide-on-med-and-down">
                       <li><a href="">{{ linkOne }}</a></li>
                       <li><a href="">{{ linkTwo }}</a></li>
                   </ul>
               </div>
           </nav>
        </div>
    </div>
</template>

<script>
export default {
    data() {
        return {
            navTitle: 'Photos',
            linkOne: 'Inicio',
            linkTwo: 'Ayuda'
        }
    }
}
</script>

<style scoped>
    .brand-logo {
        margin-left: 15px;
    }

    .nav-wrapper {
        background-color: #0d47a1;
    }
</style>
<template>
    <div>
        <ul>
            <li v-for="i in person" :key="i.name" @click="i.show = !i.show">
                <h4>Name : {{i.name}}</h4>
                <h6 v-show="i.show">Job : {{i.job}}</h6>
            </li>
        </ul>
    </div>
</template>


<script>
    export default{
        data(){
            return{
                person: [
                    {name: 'Gumiho', job: 'GameDeveloper', show: false},
                    {name: 'Hong', job: 'BackendDeveloper', show: false},
                    {name: 'Lin', job: 'FullStackDeveloper', show: false},
                    {name: 'Ly', job: 'UI/UX', show: false},
                    {name: 'Tey', job: 'FrontendDeverloper', show: false},
                    {name: 'Ma Ya', job: 'Model', show: false},
                ]
            }
        }
    }
</script>

<style scoped>
    div{
        padding: 20px;
        display: flex;
        justify-content: center;
        align-items: center;
        flex-direction: none;
    }
    ul li {
        list-style-type: none;
        display: inline-block;
        padding: 50px 30px;
        margin: 10px 20px;
        color: #333;
        border: 3px solid skyblue;
    }
    h6{
        text-align: centerS;
    }
</style>
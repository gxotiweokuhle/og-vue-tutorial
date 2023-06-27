<template>
   
        <h2>Text Input</h2>
        <input v-model="text">{{text}}
        <h2>Checkbox</h2>
        <input type="checkbox" id="checkbox" v-model="checked">
        <label for="checkbox">checked: {{checked}}</label>
        <h2>Muilti Check</h2>
        <input type="checkbox" id="luke" v-model="checkedNames" value="luke" >
        <label for="luke">Luke</label><!--second option on the list-->
        <input type="checkbox" id="cheslyn" v-model="checkedNames" value="cheslyn">
        <label for="chesyn">cheslyn</label>
        <p>Checked:
            <pre>{{ checkedNames }}</pre>
        </p>
        <h2>Radio</h2>
        <input type="radio" id="one" value="one" v-model="picked">
        <label for="one">One</label>
        <br>
        <input type="radio" id="two" value="two" v-model="picked">
        <label for="two">Two</label>
        <br>
        <span>Picked: {{ picked }}</span>
        <h2>Select</h2>
        <select v-model="muiltiSelected" multiple style="width: 100px;">
            <option >A</option>
            <option >B</option>
            <option >C</option>
        
        </select><!---muliple is a attribute to choose muiltples-->
        <br>
        <span>Selected:{{ muiltiSelected }}</span>
        
</template>
<script>
    export default{
        data(){
            return{
                text:'',
                checked: true,
                checkedNames:['cheslyn'], 
                picked:['one'],//default value
                muiltiSelected:'A',
            }
        }
    }

</script>
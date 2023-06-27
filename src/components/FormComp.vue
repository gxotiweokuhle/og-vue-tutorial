<!----<template>
   
        <h2>Text Input</h2>
        <input v-model="text"><br>{{text}}
        <h2>Checkbox</h2>
        <input type="checkbox" id="checkbox" v-model="checked">
        <label for="checkbox">checked: {{checked}}</label>
        <h2>Muilti Check</h2>
        <input type="checkbox" id="luke" v-model="checkedNames" value="luke" >
        <label for="luke">Luke</label>
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
        
        </select>
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

</script>-->
<template>
    <h5>Create a <span>Foschini</span> Account</h5>
    <form>
        <br>
        <div class="name">
            <h5>Fullname:</h5>
            <input type="name" class="form-control" id="exampleFormControlInput1" v-model="name"><br>
            {{name}}
            
        </div>
        <div class="id">
            <h5>Are you are a South African Citizen?</h5>
            <input type="radio" id="yes" v-model="confirm" value="Yes" >
            <label for="yes" class="yes">Yes</label>
            <input type="radio" id="no" v-model="confirm" value="No" >
            <label for="no" class="no">No</label>
           <br>
           <span>Confirmed:
            <pre>{{confirm}}</pre>
           </span>  
        </div>
        <div class="id">
            <h5>ID Number:</h5>
            <input type="number" class="form-control" id="exampleFormControlInput2" v-model="number"><br>
            {{number}}
        </div>
        <div class="phone">
            <h5>Phone Number:</h5>
            <input type="email" class="form-control" id="exampleFormControlInput2" v-model="idNo"><br>
            {{idNo}}
        </div>
        <div class="mb-3">
            <h5>Email:</h5>
            <input type="email" class="form-control" id="exampleFormControlInput3" placeholder="name@example.com" v-model="email"><br>
            {{email}}
        </div>
        <div class="gender">
           <h5>Gender:</h5>

           <input type="radio" class="form-control" id="female"  v-model="picked" value="female">
           <label for="female">Female</label>
            <br>
            
            <input type="radio" class="form-control" id="male" v-model="picked" value="male">
            <label for="male">Male</label>
            <br>
           
            <input type="radio" class="form-control" id="other"  v-model="picked" value="other">
            <label for="other">Other</label>
            <br>
            <span>Picked: {{picked}}</span>
        </div>
         <div class="prov">
            <h5>Select Province</h5>
            <select v-model="province"  style="width: 200px; font-size: 18px;">
                <option value="Western Cape" >Western Cape</option>
                <option value="Eastern Cape">Eastern Cape</option>
                <option value="Northern Cape">Northern Cape</option>
                <option value="North West">North West</option>
                <option value="Kwa-Zulu Natal">Kwa-Zulu Natal</option>
                <option value="Free State">Free State</option>
                <option value="Gauteng">Gauteng</option>
                <option value="Limpopo">Limpopo</option>
                <option value="Mpumalanga">Mpumalanga</option>
            </select>
            <br>
            <span>Selected Province:{{province}}</span>
        </div>
        <div>
            <h5>Occupation Level:</h5>
            <input type="radio" id="employed" v-model="checked" value="Employed" >
            <label for="Employed">Employed</label><br>
            <input type="radio" id="unemployed" v-model="checked" value="Unemployed">
            <label for="Unemployed">Unemployed</label><br>
            <span>Checked:
            <pre>{{ checked }}</pre>
            </span>

        </div>

    </form>
</template>

<script>
    export default{
        data(){
            return{
                name:'',
               confirm:'',
               number:'',
               idNo:'',
               email:'',
               picked:'yes',
                picked:'',//default value
                province:'Western Cape',
                checked:'',
            }
        }
    }

</script>

<style>

    form{
        background-color: pink;
       
    }
    span{
        color: blueviolet;
    }
    
    
</style>

<template>
    <div>
        <div>
            <label>First name</label>
            <input type="text" v-model="firstName"/>
         
        </div>
        <div>
            <label>Gender</label>
            <input type="radio" name="gender" value="male" v-model="gender"><label>Male</label>
            <input type="radio" name="gender" value="female" v-model="gender"><label>Female</label>
        </div>
        <div>
            <label>Interests:</label>
            <input type="checkbox" name="interests" value="reading" v-model="interests"><label>Reading</label>
            <input type="checkbox" name="interests" value="cycling" v-model="interests"><label>Cycling</label>
            <input type="checkbox" name="interests" value="stamp-collecting" v-model="interests"><label>Stamp Collecting</label>
        </div>
        <h2>Your particulars</h2>
        <ul>
            <li>First name: {{firstName}}</li>
            <li>Gender: {{gender}}</li>
            <li>Interests: {{interests}}</li>
            
        </ul>
    </div>
</template>

<script>
export default {
    data: function(){
        return {
            firstName:"",
            gender:"male",
            interests:[]
        }
    }
}
</script>

<style scoped>

</style>
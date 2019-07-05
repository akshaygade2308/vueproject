<template>
    <div id = "mainDiv">
        
    <div className = "signUpForm">
        <h2>Event Information</h2>
        <form id="signUpId">
            <input type = "text" v-model="eventName" placeholder="Enter the Event name" value="" description = "Please enter the event name" required>
            <br><input type = "text" placeholder="Event Description" value="" required>
            <br><input type="date" placeholder="Select the Date" required>
            <br><input type="text" placeholder="Address" required>

            <br><label for="country">
            <select>
                <option value="volvo">Select the Country</option>
                <option value="volvo">Volvo</option>
                <option value="saab">Saab</option>
                <option value="opel">Opel</option>
                <option value="audi">Audi</option>
            </select>
            </label>

            <label for = "state">
            <select>
                <option value="volvo">Select the State</option>
                <option value="volvo">Volvo</option>
                <option value="saab">Saab</option>
                <option value="opel">Opel</option>
                <option value="audi">Audi</option>
            </select>
            </label>

            <!-- <br><button type="button" class="btn btn-primary dropdown-toggle" data-toggle="dropdown">Dropdown button</button>
                <div class="dropdown-menu">
                    <a class="dropdown-item" href="#">Country1</a>
                    <a class="dropdown-item" href="#">Country2</a>
                    <a class="dropdown-item" href="#">Country3</a>
                </div> -->

            <br><div>
                <b-dropdown text="Country" >
                    <b-dropdown-item href="#">Country1</b-dropdown-item>
                    <b-dropdown-item href="#">Country2</b-dropdown-item>
                    <b-dropdown-item href="#">Country3</b-dropdown-item>
                    <b-dropdown-item href="#">Country4</b-dropdown-item>
                </b-dropdown>

                <b-dropdown>
                    <template slot="button-content">
                    State
                    </template>
                    <b-dropdown-item href="#">State1</b-dropdown-item>
                    <b-dropdown-item href="#">State2</b-dropdown-item>
                    <b-dropdown-item href="#">State3</b-dropdown-item>
                    <b-dropdown-item href="#">State4</b-dropdown-item>
                </b-dropdown>
            </div>


            <!-- <br><div class="drop">
                <v-menu open-on-hover top offset-y>
                    <template v-slot:activator="{ on }">
                        <v-btn color="primary" dark v-on="on">Dropdown</v-btn>
                    </template>

                    <v-list>
                        <v-list-tile v-for="(item, index) in items"
                            :key="index">
                            <v-list-tile-title>{{ item.title }}</v-list-tile-title>
                        </v-list-tile>
                    </v-list>
                </v-menu>
            </div> -->

            <label for="company">
                <!-- <span>Company Name</span> -->
                <input type="text" id="city" placeholder="City"/>
            </label>
            <label for="contact">
                <!-- <span>Contact Name</span> -->
                <input type="text" id="zipcode" placeholder="Zipcode"/>
            </label><br>

            <input type = "text" placeholder ="City">

            <br><input type = "text" placeholder = "Zipcode">

            <br><router-link to="/login"><button className = "buttons">Add Event</button></router-link>          
        </form>
    </div>
    </div>
</template>


<script>
export default {
    data(){
        return{
            eventName : "",
            items: [
                { title: 'Option1' },
                { title: 'Option2' },
                { title: 'Option3' },
                { title: 'Option4'}
            ]
            
        }
    },

    methods :{
        // submitForm(){
            
        // },

        // check(){
        //     if 
        // }


    }
}
</script>

<style scoped>

    div {
        flex-direction: column;
        border-radius: 5px;
        background-color: #f2f2f2;
        padding: 20px;
        }

    
    label {
        width: 200px; float: left; margin: 0 20px 0 0;
        }
    span {
        display: block; margin: 0 0 3px; font-size: 1.2em; font-weight: bold;
        }

    .signUpId{
        border: 1px solid #ccc;
        border-radius: 4px;
        box-sizing: border-box;
    }

    .drop{

    }

    input[type=text], select {
    width: 50%;
    padding: 12px 20px;
    margin: 8px 0;
    display: inline-block;
    border: 1px solid #ccc;
    border-radius: 4px;
    box-sizing: border-box;
    }

    /* input[type=email], select {
    width: 50%;
    padding: 12px 20px;
    margin: 8px 0;
    display: inline-block;
    border: 1px solid #ccc;
    border-radius: 4px;
    box-sizing: border-box;
    } */

    input[type=date], select {
    width: 50%;
    padding: 12px 20px;
    margin: 8px 0;
    display: inline-block;
    border: 1px solid #ccc;
    border-radius: 4px;
    box-sizing: border-box;
    }

    .buttons{
        padding: 12px 20px;
        background-color: black;
        color: aliceblue;
        font-size: 16px;
    }

    span.a {
        float : left;
        padding: 12px 20px;
        margin: 8px 0;
        border: 1px solid #ccc;
        border-radius: 4px;
        box-sizing: border-box;
        width: 50%;
}

</style>

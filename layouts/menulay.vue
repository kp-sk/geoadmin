<template>
    <b-navbar class="navbar header has-shadow is-primary">
        <template slot="brand">
            <b-navbar-item tag="router-link" :to="{ path: '/' }">
                <img
            src="~assets/admin1.jpeg"
            alt="admin"
            height="28"
          >
            </b-navbar-item>
        </template>
        <template slot="start">
            <b-navbar-item href="/table2">
                Users
            </b-navbar-item>
            <b-navbar-item href="/tags">
                Tag List
            </b-navbar-item><b-navbar-item  href="/notification">
                Notifications
            </b-navbar-item><b-navbar-item >
                Search
                </b-navbar-item>
            
            <b-navbar-dropdown label="Settings">
                <b-navbar-item >
                    Shut Down
                </b-navbar-item>
                
            </b-navbar-dropdown>
        
            
            
        </template>

        <template slot="end">
            <b-navbar-item tag="div"  >
                <div class="buttons" >
                    <a class="button is-primary" >
                        <strong>Log Out</strong>
                    </a>
                    
                </div>
            </b-navbar-item>
        </template>
    </b-navbar>
</template>

<template>
    <div>
     <header>
        <NuxtLink to="/">Project </NuxtLink>


       </header>

       <div>
            <slot />
       </div>
        
       <footer>
            <ul>
                <li>
                    <NuxtLink to="/">Home </NuxtLink>
                </li>
                <li>
                    <NuxtLink to="/about">About</NuxtLink>
                </li>
                <li>
                    <NuxtLink to="/products">products</NuxtLink>
                </li>
            </ul>
    
        </footer>
       
    </div>
    </template>
    
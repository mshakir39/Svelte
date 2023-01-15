<button class="button-style">
    <slot></slot>
</button>

<style>

    .button-style{

        border: none;
    width: 179px;
    height: 40px;
    color: white;
    /* padding: 12px; */
    border-radius: 2px;
    /* gap: 8px; */
    background: #000000;
    }
    
    .button-style:hover{

        background: #31343F; 
}
.button-style:focus{

background: #787D8E; 
}
</style>
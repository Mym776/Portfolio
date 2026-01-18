<script>
    let {hobby} = $props()
    
</script>

<div>
    <h3>{hobby}</h3>
    <p>
        i like this {hobby} because, i like this hobby and this hobby is imprtant because this hobby is important 
    </p>
</div>

<style>
    div {
        padding: 1%;
        display: flex;
        flex-direction: column;
        justify-content: space-between;
        background-color: grey;
        align-items: center;
        width: 15%;
        border-radius: 4%;
    }
    h3 {
        font-family: monospace;

    }
    p {
        font-family: 'Courier New', Courier, monospace;
    }
</style>
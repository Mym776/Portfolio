<script>
    let {hobby, color} = $props()
</script>

<div style="background-color: {color};">
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
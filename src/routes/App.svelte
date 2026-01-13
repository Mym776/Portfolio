<script>
    let name = $state("Mohammed")
    let other_Vals = ["an Aspiring software engineer", "an A2svian","motion designer rookie"]
    let cl = $state("black")
    let cl_Vals = ["blue", "peachpuff","black","orange"]

    function s() {
        cl = cl_Vals.shift()
        name = other_Vals.shift()
        other_Vals.push(name)
        cl_Vals.push(cl)
    }
    setInterval(() => {
        s()
    }, 3000);

</script>

<style>
    * {
        font-family: monospace;
    }
    .blue {
        color: navy;
    }
    .peachpuff {
        color: green;
    }
    .black {
        color: black;
    }
    .orange {
        color: orange;
    }
</style>

<h1>Hello, I am <span class={cl}>{name}</span></h1>
<script>
    let name = $state("Mohammed")
    let other_Vals = ["Aspiring software engineer", "A2svian","motion designer rookie"]

    function s() {
        name = other_Vals.shift()
        other_Vals.push(name)
    }
    setInterval(() => {
        s()
    }, 3000);

</script>

<h1>Hello, I am {name}</h1>
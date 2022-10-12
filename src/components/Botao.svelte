<script lang="ts">
    export let texto: string;
    export let triplo: boolean = false;
    export let duplo: boolean = false;
    export let operacao: boolean = false;
    export let destaque: boolean = false;
</script>

<button class="botao" 
    class:triplo class:duplo class:destaque class:operacao>
    {texto}
</button>

<style>
    .botao{
        flex-basis: 25%;
        margin: 0;
        border: 1px solid var(--cor-fundo);
    }

    .duplo{
        flex-basis: 50%;
    }

    .triplo{
        flex-basis: 75%;
    }

    .destaque{
        background-color: red;
        color: white;
    }

    .operacao{
        background-color: orange;
        color: white;
    }
</style>
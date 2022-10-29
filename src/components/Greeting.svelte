<script lang="ts">
    export let messages: string[];
    
    let greeting: string;

    function randomMessage() {
        greeting = messages[Math.floor(Math.random() * messages.length)];
    }

    randomMessage();
</script>

<div>
    <h3>{greeting}!</h3>
    <button on:click={randomMessage}>
        New Greeting
    </button>
</div>
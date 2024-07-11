<script lang="ts">
  export let messages: string[];

  let greeting: string = messages[0];

  function randomMessage(): void {
    greeting = messages[Math.floor(Math.random() * messages.length)];
  }
</script>

<div>
  <h3>{greeting}！ 訪問いただきありがとうございます！</h3>
  <button on:click={randomMessage}>新しい挨拶</button>
</div>

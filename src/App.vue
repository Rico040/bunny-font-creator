<script setup lang="ts">
import "@skyra/discord-components-core";
</script>

<template>
  <main id="preview">
    <discord-messages>
      <discord-message
        author="ot"
        avatar="https://dp.nea.moe/avatar/619474349845643275.png"
        roleIcon="https://cdn.discordapp.com/role-icons/1225857999956869121/fe12fdb2a0a88448e026550c5f48bece.png?size=48"
        roleColor="#dc7878"
      >
        Font preview
        <discord-header :level="1"
          >Header text,
          <discord-italic>Italicized</discord-italic></discord-header
        >
        <discord-header :level="2"
          >Header 2 text,
          <discord-italic>Sample</discord-italic></discord-header
        >
        <discord-header :level="3"
          >Header 3 text,
          <discord-italic>Sample</discord-italic></discord-header
        >
        <discord-bold>Bold</discord-bold><br />
        <discord-italic>Italic</discord-italic><br />
        <Strike>Strikethrough</Strike><br />
        <discord-underlined
          >Underlines, <discord-italic>Sample</discord-italic>
          <discord-bold
            >Text. <discord-italic>Lens Flare</discord-italic></discord-bold
          ></discord-underlined
        ><br />
        <discord-subscript
          ><discord-italic>New!</discord-italic> Subtext!
          <discord-bold
            >Oh yeah!
            <discord-italic
              >This is
              <discord-underlined>Epic!</discord-underlined></discord-italic
            ></discord-bold
          >
          •
          <discord-link
            href="https://discord.com/vanityurl/dotcom/steakpants/flour/flower/index11.html"
            target="_blank"
            >Dismiss message</discord-link
          ></discord-subscript
        ><br />
        <br />
        The quick brown fox jumps over the lazy dog<br />
        THE QUICK BROWN FOX JUMPS OVER THE LAZY DOG<br />
        <br />
        <discord-mention type="channel">playground</discord-mention> <discord-mention type="user">ot</discord-mention><br />
        <discord-mention type="role" color="#dc7878">trolley</discord-mention>
      </discord-message>
    </discord-messages>
  </main>
</template>

<style scoped>
.logo {
  height: 6em;
  padding: 1.5em;
  will-change: filter;
  transition: filter 300ms;
}
.logo:hover {
  filter: drop-shadow(0 0 2em #646cffaa);
}
.logo.vue:hover {
  filter: drop-shadow(0 0 2em #42b883aa);
}
</style>

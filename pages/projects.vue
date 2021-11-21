<template>
  <div>
    <Header links="links-Top">
      <h1>projects</h1>
    </Header>

    <h2>
      <code class="active">· active</code>
    </h2>
    <div id="cards">
      <ProjectCard>
        <template #header>Rust (for absolute beginners)</template>
        <template #body>
          <p>
            A series of recorded live tutorials where I teach absolute beginners
            <a
              href="https://rust-lang.org"
            >Rust</a>, my personal favorite general-purpose
            language. I believe that Rust, contrary to its reputation of being complex and
            requiring previous programming experience to comprehend, can be taught
            successfully to beginners, and this series is my attempt at doing so.
          </p>
        </template>
        <template #footer>
          <NuxtLink to="/rfab/what">[see more]</NuxtLink>
        </template>
      </ProjectCard>

      <ProjectCard>
        <template #header>
          Quinstaller
          <em>(temporary name)</em>
        </template>
        <template #body>
          <p>
            An all-in-one installer/interactive guide developed for RfAB that installs
            <a
              href="https://rust-lang.org"
            >Rust</a> (via
            <code>
              <a href="https://rustup.rs">rustup</a>
            </code>),
            <a href="https://code.visualstudio.com">Visual Studio Code</a> and
            <a href="https://git-scm.com/">Git</a>.
          </p>
          <p>
            Currently based on
            <a href="https://tauri.studio">Tauri</a>,
            <a href="https://vitejs.dev">Vite.js</a> and
            <a href="https://v3.vuejs.org">Vue.js 3</a> (subject to change)
          </p>
        </template>
        <template #footer>
          <a href="https://github.com/leocth/quinstaller">[github (to be made public)]</a>
        </template>
      </ProjectCard>
    </div>

    <h2>
      <code class="on-hold">~ on hold</code>
    </h2>
    <div id="cards">
      <ProjectCard>
        <template #header>Tips and Tricks</template>
        <template #body>
          <p>
            An assortment of Tips and Tricks about a variety of things, Currently mostly
            about Minecraft modding with
            <a
              href="https://quiltmc.org"
            >QuiltMC</a> and/or
            <a href="https://fabricmc.net">FabricMC</a>.
          </p>
        </template>
        <template #footer>
          <a href="https://github.com/leocth/tips-and-tricks">[github]</a>
        </template>
      </ProjectCard>
    </div>

    <h2>
      <code class="inactive">- inactive</code>
    </h2>
    <div id="cards">
      <ProjectCard>
        <template #header>Gravity Guns</template>
        <template #body>
          <p>
            A Minecraft mod that adds the Gravity Gun from Half-Life 2.
            Entry for ModFest 1.17.
          </p>
          <p>
            It only works on 1.17.x, it's buggy, it lags your computer,
            I had to coax it together before the ModFest deadline, it's
            horrible, use with caution.
          </p>
        </template>
        <template #footer>
          <ul>
            <li>
              <a href="https://github.com/leocth/gravity-guns">[github]</a>
            </li>
            <li>
              <a href="https://modrinth.com/mod/gravity-guns">[modrinth]</a>
            </li>
          </ul>
        </template>
      </ProjectCard>
      <ProjectCard>
        <template #header>Drunk Fletchin' Table</template>
        <template #body>
          <p>
            A Minecraft mod that adds some additional and questionable functions to the
            as-of-now unused Fletching Table.
          </p>
          <p>
            Published versions only target 1.16.x. A 1.17.x version was in the making
            before being abandoned.
          </p>
        </template>
        <template #footer>
          <ul>
            <li>
              <a href="https://github.com/leocth/drunk-fletchin-table">[github]</a>
            </li>
            <li>
              <a
                href="https://www.curseforge.com/minecraft/mc-mods/drunk-fletchin-table"
              >[curseforge]</a>
            </li>
          </ul>
        </template>
      </ProjectCard>
      <ProjectCard>
        <template #header>RGBable</template>
        <template #body>
          <p>
            A Minecraft mod that adds
            <span class="faaaaaaancyyyyyyy">colorful</span> blocks.
          </p>
          <p>
            Published versions only target 1.16.x. There's a copy on my computer
            that works on 1.17.x but I kinda got lazy and never published it.
          </p>
          <p>
            <del>
              Just use
              <a href="https://modrinth.com/mod/painters-blocks">Painter's Blocks</a>
              instead, Juuz is a much more competent modder than I am lol
            </del>
          </p>
        </template>
        <template #footer>
          <ul>
            <li>
              <a href="https://github.com/leocth/rgbable">[github]</a>
            </li>
            <li>
              <a href="https://www.curseforge.com/minecraft/mc-mods/rgbable">[curseforge]</a>
            </li>
          </ul>
        </template>
      </ProjectCard>
      <ProjectCard>
        <template #header>Less Annoying Piglins</template>
        <template #body>
          <p>A small Minecraft mod that makes piglins non-aggressive after bartering.</p>
          <p>Verified to work on 1.16.x., probably also works on 1.17.x.</p>
        </template>
        <template #footer>
          <ul>
            <li>
              <a href="https://github.com/leocth/LessAnnoyingPiglins">[github]</a>
            </li>
            <li>
              <a href="https://modrinth.com/mod/OhCCsdMD">[modrinth]</a>
            </li>
          </ul>
        </template>
      </ProjectCard>
      <ProjectCard>
        <template #header>
          Better
          <code>rsqrt</code>
        </template>
        <template #body>
          <p>
            An extremely small, one-mixin mod that replaces the constants Minecraft
            used in their
            <a
              href="https://en.wikipedia.org/wiki/Fast_inverse_square_root"
            >fast reciprocal square root</a> method, with supposedly more accurate
            alternatives.
          </p>
        </template>
        <template #footer>
          <ul>
            <li>
              <a href="https://github.com/leocth/better-rsqrt">[github]</a>
            </li>
            <li>
              <a href="https://modrinth.com/mod/better-rsqrt">[modrinth]</a>
            </li>
          </ul>
        </template>
      </ProjectCard>
    </div>
  </div>
</template>

<style scoped>
#cards {
  display: grid;
  grid-template-columns: repeat(auto-fill, minmax(500px, auto));
  grid-auto-rows: minmax(100px, auto);

  gap: 30px;
  margin: 50px;
}

.active {
  color: rgb(104, 245, 33);
}
.on-hold {
  color: rgb(233, 219, 23);
}
.inactive {
  color: rgb(83, 83, 83);
}

ul {
  display: flex;
  align-items: flex-end;
  padding: 0;
}
ul > li {
  display: inline-block;
  margin-right: 10px;
}

.faaaaaaancyyyyyyy {
  background: linear-gradient(
    to right,
    rgb(138, 10, 10),
    rgb(143, 97, 13),
    rgb(168, 168, 14),
    rgb(22, 133, 22),
    rgb(31, 31, 136),
    rgb(88, 27, 131)
  );
}
</style>

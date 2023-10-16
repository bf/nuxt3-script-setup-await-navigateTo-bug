# nuxt3 `await navigateTo` bug when used in <script setup>`

`await navigateTo` does not terminate `<script setup>`, execution continues. last `await navigateTo` overwrites previous ones.

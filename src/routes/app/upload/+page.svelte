<script lang="js">
  import { browser } from "$app/environment";

  $: if (browser) document.title = "Upload";
</script>

<div class="mt-72 flex justify-center">
  <div class="m-auto text-center">
    <div class="flex w-full items-center justify-center">
      <label
        for="file-dropzone"
        class="flex h-64 w-96 cursor-pointer flex-col items-center justify-center rounded-lg border-2 border-solid border-gray-300 bg-white shadow-inner hover:bg-gray-50 active:bg-gray-100"
      >
        <div class="flex flex-col items-center justify-center pt-5 pb-6">
          <svg
            aria-hidden="true"
            class="mb-3 h-10 w-10 text-gray-400"
            fill="none"
            stroke="currentColor"
            viewBox="0 0 24 24"
            xmlns="http://www.w3.org/2000/svg"
            ><path
              stroke-linecap="round"
              stroke-linejoin="round"
              stroke-width="2"
              d="M7 16a4 4 0 01-.88-7.903A5 5 0 1115.9 6L16 6a5 5 0 011 9.9M15 13l-3-3m0 0l-3 3m3-3v12"
            /></svg
          >
          <p class="mb-2 text-sm text-gray-500 dark:text-gray-400">
            <span class="font-semibold">Click to upload</span> or drag and drop
          </p>
          <p class="text-xs text-gray-500 dark:text-gray-400">
            List any file requirements here (formats, sizes, etc)
          </p>
        </div>
        <input id="file-dropzone" type="file" class="hidden" />
      </label>
    </div>
  </div>
</div>

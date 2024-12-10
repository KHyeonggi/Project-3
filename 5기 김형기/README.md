## 테일윈드 적용

-   [vite + tailwindcss](https://tailwindcss.com/docs/guides/vite)

```js
import { defineConfig } from 'vite'
import react from '@vitejs/plugin-react'
import tailwindcss from 'tailwindcss'

// https://vitejs.dev/config/
export default defineConfig({
    plugins: [react()],
    css: {
        postcss: {
            plugins: [tailwindcss()],
        },
    },
})
```
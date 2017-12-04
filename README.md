# ESLINT-CONFIG-CDRAINXV

---

`eslint-config-cdrainxv` is a **very** opinionated eslint config (or will be as
it is incrementally updated it stricter rules). This config is coupled with
**prettier** for easy formatting.

# Usage

---

1. `npm i eslint-config-cdrainxv`

2. Add peer dependencies: `npm i eslint eslint-config-prettier
   eslint-plugin-prettier prettier prettier-eslint prettier-eslint-cli -D`

3. Create `.eslintrc*` configuration file

4. include `cdrainxv` as an extention:

   **.eslintrc.js**

   ```js
   module.exports = {
     extends: ['cdrainxv']
   }
   ```

   ---

   **.eslintrc.json**

   ```json
   {
     "extends": ["cdrainxv"]
   }
   ```

5. Add lint scripts to package.json:

  ```json
    "scripts": {
      "lint": "prettier-eslint .",
      "eslint-check": "eslint --print-config .eslintrc.js | eslint-config-prettier-check"
    }
  ```

6. Configure further with your own rules and/or plugins.

7. Check that your rules don't conflict with **Prettier**'s own rules:
  `npm run eslint-check`

8. Run linter: `npm run lint`

---

## References:

[prettier/prettier](https://github.com/prettier/prettier) | 
[prettier/eslint-plugin-prettier](https://github.com/prettier/eslint-plugin-prettier) | 
[prettier/prettier-eslint](https://github.com/prettier/prettier-eslint) | 
[prettier/prettier-eslint-cli](https://github.com/prettier/prettier-eslint-cli)
| 
[eslint](https://eslint.org/docs/rules/)

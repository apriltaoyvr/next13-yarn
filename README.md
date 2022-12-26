For https://github.com/vercel/next.js/issues/44346

This issue seems to happen when Next 13 app projects are scaffolded with Yarn. I did not encounter these issues when copying over these files to the other error example template (that was created with npm).

## To Reproduce

1. Clone the yarn example
2. Run the dev server
3. It will now 404 as the `app/page.tsx` file is skipped over
4. Create `app/[slug]/page.tsx`
5. It will no longer 404 but the `app/page.tsx` file will still be skipped over

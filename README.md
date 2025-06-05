# Repro steps

1. pnpm install in individual folders
2. From root run `pnpm dlx wrangler@latest dev -c my-producer-worker/wrangler.jsonc -c my-consumer-worker/wrangler.jsonc`
3. Should then see `✘ [ERROR] Worker "core:user:my-consumer-worker"'s binding "MY_SECOND_WORKER" refers to a service "core:user:my-second-worker", but no such service is defined.` in CLI output

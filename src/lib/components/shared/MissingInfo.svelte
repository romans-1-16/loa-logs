<script lang="ts">
    import { missingInfo } from "$lib/utils/stores";
    import { tooltip } from "$lib/utils/tooltip";
</script>

{#if $missingInfo}
    <div
        class="text-left font-normal whitespace-nowrap text-red-400"
        use:tooltip={{
            content:
                "METER OPENED TOO LATE, UNABLE TO READ DAMAGE DATA. Please go to CHARACTER SELECT or SWAP CHARACTERS."
        }}>
        WARNING: INVALID DATA
    </div>
{/if}

<script>
    export let name;
    export let percent;
    export let color;
</script>
<div class="progress-wrap">
    <h3>{name}</h3>
    <div class="progress">
        <div class="progress-bar {color}" role="progressbar" aria-valuenow="{percent}"
        aria-valuemin="0" aria-valuemax="100" style="width:{percent}%">
        <span>{percent}%</span>
        </div>
    </div>
</div>
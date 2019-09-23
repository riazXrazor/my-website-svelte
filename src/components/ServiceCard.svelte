<script>
    export let icon;
    export let color;
    export let title;
    export let description;

</script>


<div class="services {color}">
    <span class="icon">
        <i class="icon-{icon}"></i>
    </span>
    <div class="desc">
        <h3>{title}</h3>
        <p>{description}</p>
    </div>
</div>
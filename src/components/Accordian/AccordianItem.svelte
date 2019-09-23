<script>
    export let title;
    export let tabId;
    export let active;
</script>
<div class="panel panel-default">
    <div class="panel-heading" role="tab" id="heading{tabId}">
        <h4 class="panel-title">
            <a data-toggle="collapse" data-parent="#accordion" href="#{tabId}">
                {title}
            </a>
        </h4>
    </div>
    <div id="{tabId}" class="panel-collapse collapse {active == true ? 'in' : ''}" role="tabpanel" aria-labelledby="heading{tabId}">
            <div class="panel-body">
                <slot></slot>
            </div>
    </div>
</div>
<script>
    import Icon from '$lib/icon.svelte';
</script>

<h1>Credits, Contact, & Contributions</h1>

<hr />

<h2 class="text-center">Site Admins</h2>

<br>

<div class="grid grid-cols-1 sm:grid-cols-2 gap-6">
    
    <div class="bg-white border shadow-sm border-gray-100 p-6 relative overflow-visible card-ripple">
        <h4 class="text-xl mb-4 leading-4">
		    canti
			<br>
			<span class="font-thin text-xs">Data Hoarder</span>
		</h4>
        
        <ul class="space-y-4">

            <li class="flex items-center gap-3">
                <div class="relative group flex items-center justify-center">
                    <Icon messenger="fluxer" />
                    <span class="pointer-events-none absolute -top-8 left-1/2 -translate-x-1/2 whitespace-nowrap rounded bg-gray-800 px-2 py-1 text-xs text-white opacity-0 group-hover:opacity-100 transition-opacity z-10">
                        Fluxer
                    </span>
                </div>
                <span class="font-medium text-sm">canti#7196</span>
            </li>
            
            <li class="flex items-center gap-3">
                <div class="relative group flex items-center justify-center">
                    <Icon messenger="discord" />
                    <span class="pointer-events-none absolute -top-8 left-1/2 -translate-x-1/2 whitespace-nowrap rounded bg-gray-800 px-2 py-1 text-xs text-white opacity-0 group-hover:opacity-100 transition-opacity z-10">
                        Discord
                    </span>
                </div>
                <span class="font-medium text-sm">cantimaru</span>
            </li>
            
        </ul>
    </div>

    <div class="bg-white border shadow-sm border-gray-100 p-6 relative overflow-visible card-ripple">
        <h4 class="text-xl mb-4 leading-4">
		    Nautichor
			<br>
			<span class="font-thin text-xs">Writer & Editor</span>
		</h4>
        
        <ul class="space-y-4">
            
            <li class="flex items-center gap-3">
                <a href="https://signal.me/#eu/rxTvzMIPHoPXPFejeR63yU-2T9ZWXTgWKVD0mfC8wRQCwFpeyl5EB5r_v0Qs_44R" target="_blank" class="flex items-center gap-3 group">
                    <div class="relative group flex items-center justify-center">
                        <Icon messenger="signal" />
                        <span class="pointer-events-none absolute -top-8 left-1/2 -translate-x-1/2 whitespace-nowrap rounded bg-gray-800 px-2 py-1 text-xs text-white opacity-0 group-hover:opacity-100 transition-opacity z-10">
                            Signal
                        </span>
                    </div>
                    <span class="font-medium text-sm">@NAUTICHOR.2424</span>
                </a>
            </li>
            
            <li>
                <a href="https://steamcommunity.com/id/NAUTICHOR" class="flex items-center gap-3 group">
                    <div class="relative flex items-center justify-center">
                        <Icon messenger="steam" />
                        <span class="pointer-events-none absolute -top-8 left-1/2 -translate-x-1/2 whitespace-nowrap rounded bg-gray-800 px-2 py-1 text-xs text-white opacity-0 group-hover:opacity-100 transition-opacity z-10">
                            Steam
                        </span>
                    </div>
                    <span class="font-medium text-sm">Nautichor</span>
                </a>
            </li>

            <li class="flex items-center gap-3">
                <div class="relative group flex items-center justify-center">
                    <Icon messenger="email" />
                    <span class="pointer-events-none absolute -top-8 left-1/2 -translate-x-1/2 whitespace-nowrap rounded bg-gray-800 px-2 py-1 text-xs text-white opacity-0 group-hover:opacity-100 transition-opacity z-10">
                        E-mail
                    </span>
                </div>
                <span class="font-medium text-sm">not yet</span>
            </li>
                     
            <li>
                <a href="https://t.me/nautichor" target="_blank" class="flex items-center gap-3 group">
                    <div class="relative flex items-center justify-center">
                        <Icon messenger="telegram" />
                        <span class="pointer-events-none absolute -top-8 left-1/2 -translate-x-1/2 whitespace-nowrap rounded bg-gray-800 px-2 py-1 text-xs text-white opacity-0 group-hover:opacity-100 transition-opacity z-10">
                            Telegram
                        </span>
                    </div>
                    <span class="font-medium text-sm">@nautichor</span>
                </a>
            </li>
			
        </ul>
    </div>

</div>

<br><hr />

<style>
    .card-ripple {
        position: relative;
    }

    .card-ripple:hover::after {
        content: '';
        position: absolute;
        inset: 0;
        border: 2px solid rgba(59, 130, 246, 0.7);
        pointer-events: none;
        animation: expand 0.15s linear infinite;
    }

    @keyframes expand {
        0% {
            transform: scale(1.00);
        }
        100% {
            transform: scale(1.02);
        }
    }
</style>
<script lang="ts">
	import { T } from '@threlte/core';
	import { OrbitControls } from '@threlte/extras';
	import { color } from 'three/tsl';
	import { MeshBasicNodeMaterial } from 'three/webgpu';
</script>

<T.PerspectiveCamera makeDefault position={[0, 0, 10]}>
	<OrbitControls />
</T.PerspectiveCamera>

<T.Mesh>
	<T.BoxGeometry />
	<T is={MeshBasicNodeMaterial} colorNode={color('#fff000')} />
</T.Mesh>

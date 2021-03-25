<script lang="ts">
  import TopAppBar, { Row, Section, Title } from '@smui/top-app-bar';
</script>

<style>
	#top-bar {
		background-color: #fff;
		color: #000;
	}
</style>

<TopAppBar variant="fixed" id="top-bar">
	<Row>
		<Section>
			<Title href="/">
				<img src="/monogram.svg" alt="tracktor monogram" height="50" style="display: inline; vertical-align: middle;"> Tracktor
			</Title>
		</Section>
	</Row>
</TopAppBar>
<script>
	import SiteHeader from '../../components/SiteHeader.svelte';
</script>

<SiteHeader />

<div class="page">
	<div class="main-table-containter">
		<div class="title-table-container">
			<div class="subtitle">Robolobos Documentation</div>
		</div>
		<div>
			<table>
				<tbody>
                    <tr>
						<td>Name</td>
						<td>Year</td>
						<td>Robot Name</td>
						<td>Link</td>
					</tr>
					<tr>
						<td>BASE_2024</td>
						<td>2024</td>
						<td>N/A</td>
						<td>
                            <a target="_blank" href="https://frc2359.github.io/BASE_2024/">Base 2024</a>
                        </td>
					</tr>
				</tbody>
			</table>
		</div>
	</div>

	<div class="main-table-containter">
		<div class="title-table-container">
			<div class="subtitle">External Documentation</div>
		</div>
		<div>
			<table>
				<tbody>
                    <tr>
						<td>Name</td>
						<td>Use</td>
						<td>Link</td>
					</tr>
					<tr>
						<td>WPILib</td>
                        <td>
                            Base funcions for FRC Robotics control
                        </td>
						<td>
                            <a target="_blank" href="https://github.wpilib.org/allwpilib/docs/release/java/index.html">WPILib API</a>
                        </td>
						
					</tr>
                    <tr>
						<td>Phoenix 6</td>
                        <td>
                            Functions to control CTRE devices
                        </td>
						<td>
                            <a target="_blank" href="https://api.ctr-electronics.com/phoenix6/release/java/">CTRE Phoenix 6 API</a>
                        </td>
					</tr>
                    <tr>
						<td>REV Robotics</td>
                        <td>
                            Functions to control REV Robotics devices
                        </td>
						<td>
                            <a target="_blank" href="https://codedocs.revrobotics.com/java/com/revrobotics/package-summary.html">REV API</a>
                        </td>
					</tr>
                    <tr>
						<td>Limelight</td>
                        <td>
                            Information, functions, and setup of Limelight
                        </td>
						<td>
                            <a target="_blank" href="https://docs.limelightvision.io/docs/docs-limelight/getting-started/summary">Limelight Docs</a>
                        </td>
					</tr>
				</tbody>
			</table>
		</div>
	</div>
</div>

<style>
	.page {
		margin-top: 15vh;
		padding-left: 2vw;
        font-family: 'Work Sans', 'Helvetica', 'sans-serif';
	}

    a {
        color: green;
    }

	.main-table-containter {
		border-radius: 20px;
		background-color: #474747;
		width: 90vw;
		padding: 1rem 1rem;
		box-shadow: 0px 2px 5px 0px #00000033;
        margin-top: 2vh;
	}

	.title-table-container {
		display: flex;
		justify-content: space-between;
		margin-bottom: 1.2rem;
		align-items: center;
		padding-top: 2em;
		padding-bottom: 3em;
	}

	.subtitle {
		font-weight: 900;
        font-size: 3vh;
		font-family: 'Rockwell', 'Arvo', 'sans-serif';
	}

	table {
		width: 100%;
		font-weight: 600;
		font-size: 1.5vh;
		border-collapse: collapse;
		color: white;
	}

	tr {
		border-radius: 20px;
		transition: background-color 0.2s;
	}
	tr:hover {
		background-color: #171717;
	}
	td {
		padding: 1rem;
		border: none;
	}

	td {
		text-align: left;
	}
	td:first-child {
		border-radius: 1.5rem 0rem 0rem 1.5rem;
		text-align: left;
	}

	td:last-child {
		border-radius: 0rem 1.5rem 1.5rem 0rem;
	}
</style>

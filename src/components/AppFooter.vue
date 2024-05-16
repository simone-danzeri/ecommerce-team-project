<script>
export default {
	name: "AppFooter",
	props: {
		footerKnowLinks: Array,
		footerEarnLinks: Array,
		footerPaymentsLinks: Array,
		footerHelpLinks: Array,
		footerCountries: Array,
	},
	data() {
		return {};
	},
	methods: {
		scrollToTop() {
			window.scrollTo({ top: 0, behavior: "smooth" });
		},
	},
};
</script>

<template>
	<div class="container">
		<div class="ms-footer-top-container d-flex justify-content-around py-4">
			<!-- Conoscersi meglio -->
			<div class="ms-get-to-know-links">
				<ul>
					<li class="text-white fw-bold">Conoscersi Meglio</li>
					<li v-for="eachLink in footerKnowLinks" class="py-2">
						<a class="fw-lighter" href="#">{{ eachLink }}</a>
					</li>
				</ul>
			</div>
			<!-- Guadagna con Amazon -->
			<div class="ms-earn-links">
				<ul>
					<li class="text-white fw-bold">Guadagna con Amazon</li>
					<li v-for="eachLink in footerEarnLinks" class="py-2">
						<a class="fw-lighter" href="#">{{ eachLink }}</a>
					</li>
				</ul>
			</div>
			<!-- Metodi di pagamento -->
			<div class="ms-payments-links">
				<ul>
					<li class="text-white fw-bold">Metodi di pagamento</li>
					<li v-for="eachLink in footerPaymentsLinks" class="py-2">
						<a class="fw-lighter" href="#">{{ eachLink }}</a>
					</li>
				</ul>
			</div>
			<!-- Bisogno di aiuto -->
			<div class="ms-help-links">
				<ul>
					<li class="text-white fw-bold">Hai bisogno di aiuto?</li>
					<li v-for="eachLink in footerHelpLinks" class="py-2">
						<a class="fw-lighter" href="#">{{ eachLink }}</a>
					</li>
				</ul>
			</div>
		</div>
		<!-- Bottone per tornare in top??? -->
		<div class="ms-back-top d-flex justify-content-center align-items-center" @click="scrollToTop()">
			<!-- altezza fissa -->
			<span class="fw-light">Torna su</span>
		</div>
		<!-- Sezione mid del footer con logo e lista paesi -->
		<section class="ms-mid-footer">
			<div class="ms-hr"></div>
			<div class="ms-logo-footer-container d-flex justify-content-center py-4">
				<img src="../assets/img/amazon-logo.jpg" alt="..." />
			</div>
			<div class="ms-country-list-container py-4">
				<ul class="d-flex justify-content-center flex-wrap">
					<li v-for="eachCountry in footerCountries" class="mx-3 pb-2">
						<a class="fw-lighter" href="#">{{ eachCountry }}</a>
					</li>
				</ul>
			</div>
		</section>
	</div>
</template>

<style scoped lang="scss">
@use "../style/partials/variables" as *;

.ms-footer-top-container {
	background-color: $secondary-color;

	ul {
		list-style: none;

		li {
			list-style: none;

			a {
				text-decoration: none;
				color: $white;
			}
		}
	}
}

.ms-back-top {
	background-color: #37475b;
	height: 50px;
	min-width: 100%;
	color: $white;
	cursor: pointer;

	&:hover {
		opacity: 0.95;
	}

	span {
		font-size: 14px;
	}
}

.ms-mid-footer {
	background-color: $secondary-color;

	.ms-hr {
		border: 1px solid #3a4553;
	}

	.ms-logo-footer-container {
		margin: 0 auto;

		img {
			max-width: 8%;
		}
	}
}

.ms-country-list-container {
	ul {
		list-style: none;
		margin-left: -32px;

		li {
			list-style: none;

			a {
				text-decoration: none;
				color: $white;
			}
		}
	}
}
</style>

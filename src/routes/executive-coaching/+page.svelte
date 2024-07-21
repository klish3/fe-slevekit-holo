<script lang="ts">
	import { ArrowRightOutline } from 'flowbite-svelte-icons';
	import { Section, HeroHeader, FeatureDefault, FeatureItem, Cta } from 'flowbite-svelte-blocks';
	import {
		LandmarkSolid,
		BriefcaseSolid,
		DollarOutline,
		RocketSolid,
		CogOutline
	} from 'flowbite-svelte-icons';
</script>

<Section name="ctawithimg">
	<Cta ctatype="image">
		<svelte:fragment slot="img">
			<img
				class="w-full dark:hidden"
				src="https://flowbite.s3.amazonaws.com/blocks/marketing-ui/cta/cta-dashboard-mockup.svg"
				alt="dashboard"
			/>
			<img
				class="hidden w-full dark:block"
				src="https://flowbite.s3.amazonaws.com/blocks/marketing-ui/cta/cta-dashboard-mockup-dark.svg"
				alt="dashboard"
			/>
		</svelte:fragment>
		<svelte:fragment slot="h2"
			>Let's create more tools and ideas that brings us together.</svelte:fragment
		>
		<p class="mb-6 font-light text-gray-500 dark:text-gray-400 md:text-lg">
			Flowbite helps you connect with friends and communities of people who share your interests.
			Connecting with your friends and family as well as discovering new ones is easy with features
			like Groups.
		</p>
		<!-- <a
			href="/"
			class="inline-flex items-center rounded-lg bg-primary-700 px-5 py-2.5 text-center text-sm font-medium text-white hover:bg-primary-800 focus:ring-4 focus:ring-primary-300 dark:focus:ring-primary-900"
		>
			Get started
			<ArrowRightOutline size="md" class="-mr-1 ml-2" />
		</a> -->
	</Cta>
</Section>

<Section name="feature">
	<HeroHeader
		class="mb-8 max-w-screen-md lg:mb-16"
		h2Class="mb-4 text-4xl tracking-tight font-extrabold text-gray-900 dark:text-white"
		pClass="text-gray-500 sm:text-xl dark:text-gray-400"
	>
		<svelte:fragment slot="h2">Bio</svelte:fragment>
		<svelte:fragment slot="paragraph">
			<p>
				Brian has worked in corporate for over 30 years. During this time he has operated from the
				customer-facing frontline, to company Director Level, and has worked in Manufacturing,
				Business-to- industrial consumer marketing with AECI and Group 5, and in the financial
				services sector with Nedcor, where he rose to the level of Divisional Director. Brain has
				operated in South Africa, sub-Saharan Africa, the Far East (Hong Kong and Singapore) and in
				the Middle East.
			</p>
			<p>
				Brian heads up Holon Management Consulting. A business consulting unit that focuses on
				enabling organizations improve operational efficiencies and bottom line profitability
				through the following:
			</p>
		</svelte:fragment>
	</HeroHeader>
	<FeatureDefault>
		<FeatureItem>
			<svelte:fragment slot="icon"
				><LandmarkSolid class="text-primary-600 dark:text-primary-300" /></svelte:fragment
			>
			<svelte:fragment slot="h3">Marketing</svelte:fragment>
			<svelte:fragment slot="paragraph"
				>Plan it, create it, launch it. Collaborate seamlessly with all the organization and hit
				your marketing goals every month with our marketing plan.</svelte:fragment
			>
		</FeatureItem>
		<FeatureItem>
			<svelte:fragment slot="icon"
				><LandmarkSolid class="text-primary-600 dark:text-primary-300" /></svelte:fragment
			>
			<svelte:fragment slot="h3">Legal</svelte:fragment>
			<svelte:fragment slot="paragraph"
				>Protect your organization, devices and stay compliant with our structured workflows and
				custom permissions made for you.</svelte:fragment
			>
		</FeatureItem>
		<FeatureItem>
			<svelte:fragment slot="icon"
				><BriefcaseSolid class="text-primary-600 dark:text-primary-300" /></svelte:fragment
			>
			<svelte:fragment slot="h3">Business Automation</svelte:fragment>
			<svelte:fragment slot="paragraph"
				>Auto-assign tasks, send Slack messages, and much more. Now power up with hundreds of new
				templates to help you get started.</svelte:fragment
			>
		</FeatureItem>
		<FeatureItem>
			<svelte:fragment slot="icon"
				><DollarOutline class="text-primary-600 dark:text-primary-300" /></svelte:fragment
			>
			<svelte:fragment slot="h3">Finance</svelte:fragment>
			<svelte:fragment slot="paragraph"
				>Audit-proof software built for critical financial operations like month-end close and
				quarterly budgeting.</svelte:fragment
			>
		</FeatureItem>
		<FeatureItem>
			<svelte:fragment slot="icon"
				><RocketSolid class="text-primary-600 dark:text-primary-300" /></svelte:fragment
			>
			<svelte:fragment slot="h3">Enterprise Design</svelte:fragment>
			<svelte:fragment slot="paragraph"
				>Craft beautiful, delightful experiences for both marketing and product with real
				cross-company collaboration.</svelte:fragment
			>
		</FeatureItem>
		<FeatureItem>
			<svelte:fragment slot="icon"
				><CogOutline class="text-primary-600 dark:text-primary-300" /></svelte:fragment
			>
			<svelte:fragment slot="h3">Operations</svelte:fragment>
			<svelte:fragment slot="paragraph"
				>Keep your company’s lights on with customizable, iterative, and structured workflows built
				for all efficient teams and individual.</svelte:fragment
			>
		</FeatureItem>
	</FeatureDefault>
</Section>

<main class="home">
	<div class="container">
		<img class="hero" src="/images/illustration-hero.svg" alt="">
		<h1 class="heading">Order Summary</h1>
		<div class="text">
			You can now listen to millions of songs, audiobooks, and podcasts on any device anywhere you like!
		</div>
		<div class="price_box">
			<div class="price_sec">
				<img class="music" src="/images/icon-music.svg" alt="">
				<div class="col">
					<div class="plan">Annual Plan</div>
					<div class="price">
						$59.99/year
					</div>
				</div>
			</div>
			<div class="change">Change</div>
		</div>
		<div class="proceed">Proceed to Payment</div>
		<div class="cancel">Cancel Order</div>
	</div>
</main>

<style>
	.home {
		@apply bg-[url('/images/pattern-background-desktop.svg')] bg-[#e0e8ff] bg-contain bg-no-repeat w-screen h-screen flex justify-center items-center;
	}
	.container {
		@apply flex flex-col w-[450px] h-[700px] items-center rounded-[20px] bg-[#ffffff];
		box-shadow: 0 15px 25px 0 hsla(245, 75%, 52%, .11);
	}
	.hero {
		@apply w-[100%] h-[225px] rounded-tl-[20px] rounded-tr-[20px] object-cover;
	}
	.heading {
		@apply mt-[42px] mb-[18px] text-[28px] text-[#1f2f56] font-extrabold;
	}
	.text {
		@apply text-[#7280a7] text-[16px] pl-[48px] pr-[48px] text-center mb-[24px] font-medium;
	}
	.price_box {
		@apply w-[344px] h-[96px] p-[24px] flex flex-row justify-between items-center bg-[#f5f7ff] rounded-[10px];
	}
	.price_sec {
		@apply flex flex-row;
	}
	.col {
		@apply flex flex-col;
	}
	.plan {
		@apply text-[18px] text-[#1f2f56] font-bold; 
	}
	.price {
		@apply text-[#7280a7] text-[16px] font-medium;
	}
	.change {
		@apply text-[16px] text-[#3829e0] font-bold cursor-pointer duration-300;
	}
	.change:hover {
		@apply underline;
	}
	.music {
		@apply w-[48px] h-[48px] mr-[12px];
	}
	.proceed {
		@apply mt-[32px] w-[350px] h-[50px] flex justify-center items-center bg-[#3829e0] text-[#ffffff] text-[16px] font-bold duration-300 rounded-[10px] cursor-pointer; 
	}
	.proceed:hover {
		@apply bg-[#3325cc];
	}
	.cancel {
		@apply text-[16px] text-[#7280a7] font-bold mt-[24px] duration-300 cursor-pointer;
	}
	.cancel:hover {
		@apply text-[#1f2f56];
	}
	@media only screen and (max-width: 450px) {
		.container {
			width: calc(100% - 32px);
		}
		.text {
			padding-left: 16px;
			padding-right: 16px;
		}
		.price_box, .proceed {
			width: calc(100% - 32px);
		}
		.price_box {
			padding-left: 16px;
			padding-right: 16px
		}
	}
	@media only screen and (max-width: 350px) {
		.music {
			width: 36px;
			height: 36px;
		}
		.plan {
			font-size: 17px;
		}
		.price, .change {
			font-size: 15px;
		}
	}
</style>
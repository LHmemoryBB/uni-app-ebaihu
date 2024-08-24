<template>
	<view class="login-page">
		<div class="page-text">
			<p class="hello-text">Hello!</p>
			<p class="slogan">欢迎登录白狐易卡</p>
		</div>
		<div class="login-form">
			<input class="uni-input" focus placeholder="账号" />
			<input class="uni-input" focus placeholder="密码" />
			<button type="primary">登录</button>
			<button class="reg-btn">注册新用户</button>
			<label class="radio">
				<radio value="r1" checked="true" />
				我已阅读并同意《用户协议》、《隐私协议》
			</label>
		</div>
	</view>
</template>

<script setup>
</script>

<style scoped lang="scss">
	.login-page {
		height: 100vh;
		width: 100%;
		position: relative;
		background-image: url('../../static/login-bg.png');
		background-size: 100% auto;
		background-repeat: no-repeat;
		overflow: hidden;

		.page-text {
			height: 400rpx;
			position: absolute;
			display: flex;
			flex-direction: column;
			justify-content: center;
			.hello-text{
				font-size: 60rpx;
				font-weight: 600;
			}
			.slogan{
				font-size: 40rpx;
			}
		}

		.login-form {
			margin-top: 400rpx;
			padding: 0 40rpx;

			input {
				background-color: #FFF;
				height: 100rpx;
				margin: 30rpx 0;
				padding-left: 20rpx;
				border-radius: 20rpx;
			}

			button {
				font-weight: 700;
				background: #488eff;
				color: #fff;
				height: 100rpx;
				margin: 30rpx 0;
				line-height: 100rpx;
				border-radius: 20rpx;
			}

			.reg-btn {
				background-color: #FFF;
				border: 1px solid #198cfe;
				color: #488eff;
			}

			.radio {

				font-size: 24rpx;

			}

			::v-deep .uni-radio-input {
				width: 28rpx;
				height: 28rpx;
			}
		}
	}
</style>
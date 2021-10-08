<template>
	<view class="content">
		<!-- <image class="logo" src="/static/logo.png"></image> -->
		<!-- 	<view class="text-area">
			<text class="title">{{title}}</text>
		</view> -->
		<u-grid class="u-padding-20" :col="3" @click='skillJump'>
			<u-grid-item index='Sword'>
				<u-icon name="photo" :size="46"></u-icon>
				<view class="grid-text">Sword</view>
				<view class="grid-text">剑盾</view>
			</u-grid-item>
			<u-grid-item index='Rapier'>
				<u-icon name="photo" :size="46"></u-icon>
				<view class="grid-text">Rapier</view>
				<view class="grid-text">西洋剑</view>
			</u-grid-item>
			<u-grid-item index='Hatchet'>
				<u-icon name="photo" :size="46"></u-icon>
				<view class="grid-text">Hatchet</view>
				<view class="grid-text">单手斧</view>
			</u-grid-item>
			<u-grid-item index='Spear'>
				<u-icon name="photo" :size="46"></u-icon>
				<view class="grid-text">Spear</view>
				<view class="grid-text">长矛</view>
			</u-grid-item>
			<u-grid-item index='Great Axe'>
				<u-icon name="photo" :size="46"></u-icon>
				<view class="grid-text">Great Axe</view>
				<view class="grid-text">双手斧</view>
			</u-grid-item>
			<u-grid-item index='War Hammer'>
				<u-icon name="photo" :size="46"></u-icon>
				<view class="grid-text">War Hammer</view>
				<view class="grid-text">战锤</view>
			</u-grid-item>
			<u-grid-item index='Bow'>
				<u-icon name="photo" :size="46"></u-icon>
				<view class="grid-text">Bow</view>
				<view class="grid-text">弓</view>
			</u-grid-item>
			<u-grid-item index='Musket'>
				<u-icon name="photo" :size="46"></u-icon>
				<view class="grid-text">Musket</view>
				<view class="grid-text">火枪</view>
			</u-grid-item>
			<u-grid-item index='Fire Staff'>
				<u-icon name="photo" :size="46"></u-icon>
				<view class="grid-text">Fire Staff</view>
				<view class="grid-text">火焰法杖</view>
			</u-grid-item>
			<u-grid-item index='Life Staff'>
				<u-icon name="photo" :size="46"></u-icon>
				<view class="grid-text">Life Staff</view>
				<view class="grid-text">生命法杖</view>
			</u-grid-item>
			<u-grid-item index='Ice Gauntlet'>
				<u-icon name="photo" :size="46"></u-icon>
				<view class="grid-text">Ice Gauntlet</view>
				<view class="grid-text">冰手套</view>
			</u-grid-item>
		</u-grid>
	</view>

</template>

<script>
	export default {
		data() {
			return {
				title: 'New World 模拟',
				weapon: [{
					name: 'Sword(剑盾)'
				}]
			}
		},
		onLoad() {

		},
		methods: {
			skillJump(index) {
				console.log(index);
				if (index === 'Life Staff') {
					this.$u.route('/pages/LifeStaff/LifeStaff');
				}
				if (index === 'Sword') {
					this.$u.route('/pages/Sword/Sword');
				}
			}
		}
	}
</script>

<style scoped lang="scss">
	.grid-text {
		font-size: 28rpx;
		margin-top: 4rpx;
		color: $u-type-info;
	}

	.content {
		display: flex;
		flex-direction: column;
		align-items: center;
		justify-content: center;
	}

	.logo {
		height: 200rpx;
		width: 200rpx;
		margin-top: 200rpx;
		margin-left: auto;
		margin-right: auto;
		margin-bottom: 50rpx;
	}

	.text-area {
		display: flex;
		justify-content: center;
	}

	.title {
		font-size: 36rpx;
		color: #8f8f94;
	}
</style>

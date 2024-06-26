1.安全efuse控制器

	propt[1]为1——non-secure操作，为0——secure操作

					offset                      non-secure                                             secure

	bank_i          0x0i0-0x000+0x10*i-1        efuse_wlock0[i]为1不可写，为0可写(rlock0同理)            efuse_wlock1[i]为1不可写，为0可写(rlock1同理)



2.eFuse和otp区别

	otp：   初始未击穿态——0

			击穿态——1

	eFuse： 初始导通——1

			熔断——0

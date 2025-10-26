	字符测试函数
		函数名	 如果是下列参数时 返回值为真
		isalnum() 字母数字（字母或数字）
		isalpha() 字母
		isblank() 标准的空白字符 
				'' > ASCII:32
				'\t' > ASCII:9
		iscntrl() 控制字符
				'\n' > ASII:10
				'\r' > ASII:13
				'\b' > ASII:8
				'\t' > ASII:9
				Ctrl+A > AASII:1
				Ctrl+B > AASII:2
		isdigit() 数字
		isgraph() 除空格之外的任意可打印字符
		islower() 小写字母
		isprint() 可打印字符
		ispunct() 标点符号（除空格字母数字以外的任何可打印字符）
		isspace() 空白字符
				isspace(' ') -> 返回真
				isspace('\n') -> 返回真
				isspace('a') -> 返回假
		isupper() 大写字母
		isxdigit() 十六进制数字符
				isxdigit('3') -> 返回真
				isxdigit('A') -> 返回真
				isxdigit('a') -> 返回真
				isxdigit('g') -> 返回假
				isxdigit('$') -> 返回假
	字符映射函数
		函数名 行为
		tolower() 如果参数是大写字符 该函数返回小写字符 否则返回原始参数
		toupper() 如果参数是小写字符 该函数返回大写字符 否则返回原始参数
from random import randint
while True:

	print("nhập: kéo, búa, bao, súng")

	player = input()
	bot = randint(0,2)

	if bot == 0:
		bot = "búa"
	if bot == 1:
		bot = "kéo"
	if bot == 2:
		bot = "bao"
	if bot == 3:
		bot = "súng"

	print("^_____^")
	print("You choose : " + player)
	print("bot choose:" + bot)
	print(">_<")

	if player == bot:
		print("hòa")
		
	else:
		if player == "kéo":
			if bot == "búa" or "súng":
				print("thất bại")
			else:
				print("WINER")

		elif player == "búa":
			if bot == "bao":
				print("thất bại")
			else:
				print("WINER")	

		elif player == "bao":
			if bot == "kéo" or "súng":
				print("thất bại")
			else:
				print("WINER")

		elif player == "súng":
			if bot == "búa":
				print("thất bại")
			else:
				print("WINER")	
		elif player == "thoát":
			break

		else:
			print("hình như có gì đó sai sai😕😕")

【このプログラムについて】

	（日本国）国土地理院版地図タイル「地理院タイル」をローカルに保存するために作成されました。
	オフラインで閲覧する用途を想定しています。

【実行に必要なファイル】

	01_iwm_GetGsiMapList.exe (.NET Desktop Runtime 10)
	02_iwm_Gsimapdl-supporter.exe (.NET Desktop Runtime 10)
	iwm_gsimapdl.exe (.NET Runtime 10 / Windows)
	iwm_gsimapdl.bin (.NET Runtime 10 / Linux)
		https://dotnet.microsoft.com/ja-jp/download/dotnet/10.0

【ファイルの説明／使用順】

	01_dl_supporter2.html
		ダウンロードしたい地理院タイルの範囲を選択し、設定ファイル（例：sample.gtsv）を取得するためのツール。

	01_iwm_GetGsiMapList.exe
		(オプションツール)
		地理院タイル種を検索。

	02_iwm_Gsimapdl-supporter.exe
		地理院タイルをダウンロードするためのGUIフロントエンド。

	iwm_gsimapdl.exe
		地理院タイルをダウンロードするためのコマンドライン・ツール。
			$ iwm_gsimapdl.exe sample.gtsv -test
		02_iwm_Gsimapdl-supporter.exe のバックエンド。

	iwm_gsimapdl.bin
		iwm_gsimapdl.exe のLinux版コマンドライン・ツール。
			$ ./iwm_gsimapdl.bin ./sample.gtsv -test

	03_dl_checker2.html
		ダウンロードされた地理院タイルを閲覧するためのオンライン版ツール。

	03_dl_checker2_offline.html
		03_dl_checker2.html のオフライン版ツール。

【主に使用するファイル】

	・Windows
		(1) 01_dl_supporter2.html
		(2) 02_iwm_Gsimapdl-supporter.exe
		(3) 03_dl_checker2.html

	・Linux
		(1) 01_dl_supporter2.html
		(2) iwm_gsimapdl.bin
		(3) 03_dl_checker2.html

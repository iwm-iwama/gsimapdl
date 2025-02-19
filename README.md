【このプログラムについて】

	（日本国）国土地理院版地図タイル「地理院タイル」をローカルに保存するために作成されました。
	オフラインで閲覧する用途を想定しています。

【実行に必要なファイル】

	01_iwm_GetGsiMapList.exe
	02_iwm_Gsimapdl-supporter.exe
	iwm_gsimapdl.exe
		Microsoft(R) .NET Framework 4.8.1 ランタイム
			https://dotnet.microsoft.com/ja-jp/download/dotnet-framework/thank-you/net481-web-installer

	iwm_gsimapdl-mono_linux.bin
		Linux Mono 環境
			https://www.mono-project.com/download/stable/#download-lin-debian
		必要なライブラリ
			libmono-system-net-http4.0-cil

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

	iwm_gsimapdl-mono_linux.bin
		iwm_gsimapdl.exe の Linux Mono 版コマンドライン・ツール。
			$ mono ./iwm_gsimapdl-mono_linux.bin ./sample.gtsv -test

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
		(2) iwm_gsimapdl-mono_linux.bin
		(3) 03_dl_checker2.html

# プログラミング講義での AI 利用（2025 春）

## 1. ソフトウェアエンジニアリングと AI
ソフトウェアエンジニアリング分野において、AI 技術の活用はますます重要になっている。とくに、**大規模言語モデル**（**LLM**（エルエルエム）: Large Language Model）と呼ばれる技術の発展により、プログラミングを支援する多様な AI ツールが登場している。プログラミング関連の AI は、その機能や目的によって、おもに次の 3 つのタイプに分類できる。

### ① コンテンツ生成、質問応答
ユーザーの入力**（プロンプト）**に基づき、文章やコード、図表、画像などのコンテンツを生成する。推論や Web 検索を活用する AI は複雑な問題にも対応できる。

| サービス名 | 開発元 | 説明 |
| --- | --- | --- |
| [**ChatGPT** :material-open-in-new:](https://chatgpt.com/){:target="_blank"}<br>（チャット・ジーピーティー） | OpenAI<br>（オープンエーアイ） | 文章生成や情報提供に優れた AI チャットボット |
| [**Claude** :material-open-in-new:](https://www.anthropic.com/claude){:target="_blank"}<br>（クロード） | Anthropic<br>（アンソロピック） | ChatGPT と同様に、会話やコンテンツ作成に特化した AI チャットボット |
| [**Grok** :material-open-in-new:](https://grok.com/){:target="_blank"}<br>（グロック） | xAI<br>（エックスエーアイ） | X（旧 Twitter）プラットフォームのデータの活用に強みを持つ AI チャットボット |
| [**Gemini** :material-open-in-new:](https://gemini.google.com/){:target="_blank"}<br>（ジェミニ） | Google<br>（グーグル） | Google が開発・提供する AI チャットボット |


### ② コーディング支援
プログラミングの学習や開発作業を効率化し、品質を高めるための AI ツール。エディタに統合され、文脈（プロジェクト全体や開いているファイル）を理解した上でのリアルタイムな支援が得意。コードの自動補完、生成、エラーチェック、ドキュメント作成などをサポートする。

| サービス名 | 開発元 | 説明 |
| --- | --- | --- |
| [**GitHub Copilot** :material-open-in-new:](https://github.com/features/copilot){:target="_blank"}<br>（ギットハブ・コパイロット） | GitHub<br>（ギットハブ） | コーディング中に AI がコードをリアルタイムで提案・自動生成するエディタ拡張機能。単純作業の自動化や新しい書き方の学習に役立つ |
| [**Cursor** :material-open-in-new:](https://www.cursor.com){:target="_blank"}<br>（カーソル） | Cursor<br>（カーソル） | AI 機能を深く統合したコードエディタ。自然言語による指示でコード生成・編集・デバッグが可能。プロジェクト全体のコードを理解し、複雑なタスクや対話的な開発を支援 |


### ③ 自律型 AI エージェント
特定の目標達成のために、複数のタスクを自律的に遂行する AI システム。ユーザーの指示がなくても、状況に応じて最適な行動を選択して実行する。発展途上の実験的な技術であり、まだ安定性や実用性の面では課題が多い。今後の進化が期待される。

| サービス名 | 開発元 | 説明 |
| --- | --- | --- |
| **Cline**<br>（クライン） | Cline<br>（クライン） | プロジェクト内のファイルを直接作成・編集し、エラーなどを監視しながら、問題を自動的に修正するコーディングエージェント |
| **Devin**<br>（デヴィン） | Cognition AI<br>（コグニション・エーアイ） | タスク指示に対して、自律的に計画を立て、コードの作成、デバッグ、問題解決をおこなうエージェント |


## 2. 推論と Web 検索機能
**推論**や **Web 検索**の機能を持っているかどうかは、AI の回答の質を大きく左右する。

### ① 推論（Reasoning: リーズニング）
複雑な問題に対して段階的に考え、論理的な推論をおこなう能力。分析や論理的思考の過程がユーザに提示される場合が多い。

!!!failure "推論機能がない場合"
	- 複雑な問題を段階的に分析せず、表面的な回答しか提供できない
	- 「なぜそうなるのか」という因果関係の説明や、複雑なコードロジックの分析が不十分になる

### ② Web 検索
生成 AI がリアルタイムでインターネット上の情報にアクセスする能力。出典となった Web ページの情報がユーザに提示される場合が多い。

!!!failure "Web 検索機能がない場合"
	- 学習データの時点**（カットオフ日）**までの情報しか持たないため、最新の技術情報やニュースを参照できない
	- 最新情報による事実確認ができないため、事実と異なる生成内容**（ハルシネーション）**を修正・検証できず、そのまま回答する可能性が高まる
	- 学習済みのデータに存在する偏りがそのまま回答に反映され、客観性に欠けた情報が提供される
	- 専門的情報やマイナーなトピックについての詳しい情報が提供されない
	- AI が提供した情報の出典をユーザが確認できず、情報の信頼性の検証が困難になる


## 3. 学生向けの無料・安価な AI ツール（2025 年 3 月現在）
- **ChatGPT**
	- 下位モデルを無料で利用可能（時間あたりの利用回数に制限あり）
	- 高性能なモデルを利用できる ChatGPT Plus プランは 20 ドル/月
- **Claude**
	- 下位モデルを無料で利用可能（時間あたりの利用回数に制限あり）
	- 高性能なモデルを利用できる Claude Pro プランは 20 ドル/月
- **Grok**
	- 最新モデル Grok 3 を無料で利用可能（時間あたりの利用回数に制限あり）
	- 将来的に有料プランが提供され、無料での利用が制限される可能性あり
- **Gemini**
	- 無料で利用可能（高性能なモデルは時間あたりの利用回数に制限あり）
	- 高性能なモデルを利用できるプランは 2,900 円/月
- **GitHub Copilot**
	- GitHub の学生開発者向けプラン（GitHub Education）に無料登録すると、無制限に利用可能

!!!warning "偽のサービスに注意"
	- インターネット上には、これらのサービス名をかたる偽のアプリや Web サイトが存在する
	- 個人情報が不正に収集されたり、料金に見合わない低性能なモデルが提供される可能性がある
	- 公式のサービスであるかを十分に確認すること


## 4. プログラミングに関するプロンプトの書き方

### ① コードブロックを使う
- プロンプトにコードを含める場合、バッククォート（\`）を使った**コードブロック**が効果的
	- 単一行のコード: 始めと終わりにバッククォートを 1 つずつ使う
	- 複数行のコード: 始めと終わりにバッククォートを 3 つずつ使う
- コードの境界が明確になり、AI の理解を助け、回答の質を向上させる
- 複数行の場合、**開始部分で言語を指定できる**
	- C 言語の場合は `c`, C++ の場合は `cpp`, Python の場合は `python`
	- 書き方は以下の「例 1」「例 2」を参照
	- AI が意図とは異なるプログラミング言語として解釈することを防げる
	- とくに C 言語は C++ と似た構文を持つため、AI が誤解する可能性が高い
- ほとんどの AI ツールは、コードブロックを視覚的にわかりやすく表示するため、人間にとっても読みやすくなる

#### 例 1

=== "🤔 コードブロックを使わない"
	````txt title="プロンプト"
	次のコードの \n は何を意味する？

	#include <stdio.h>

	int main(void)
	{
		printf("Hello, World!\n");
	}
	````

=== "✅ コードブロックを使う"
	````txt title="プロンプト" hl_lines="1 3 10"
	次のコードの `\n` は何を意味する？

	```c
	#include <stdio.h>

	int main(void)
	{
		printf("Hello, World!\n");
	}
	```
	````

#### 例 2

=== "🤔 コードブロックを使わない"
	````txt title="プロンプト"
	次のコードと同じ機能・出力結果になるように、C 言語のコードを完成させて。

	def sum_array(arr):
		total = 0
		for num in arr:
			total += num
		return total

	numbers = [5, 10, 15, 20, 25]
	result = sum_array(numbers)
	print(f"合計: {result}")

	#include <stdio.h>

	// 配列の合計を計算する関数
	int SumArray(int arr[], int size)
	{
		// ここにコードを追加
	}

	int main(void)
	{
		int numbers[] = {5, 10, 15, 20, 25};
		int size = 5;
		
		int result = SumArray(numbers, size);
		printf("合計: %d\n", result);
	}
	````

=== "✅ コードブロックを使う"
	````txt title="プロンプト" hl_lines="3 13 15 32"
	次のコードと同じ機能・出力結果になるように、C 言語のコードを完成させて。

	```python
	def sum_array(arr):
		total = 0
		for num in arr:
			total += num
		return total

	numbers = [5, 10, 15, 20, 25]
	result = sum_array(numbers)
	print(f"合計: {result}")
	```

	```c
	#include <stdio.h>

	// 配列の合計を計算する関数
	int SumArray(int arr[], int size)
	{
		// ここにコードを追加
	}

	int main(void)
	{
		int numbers[] = {5, 10, 15, 20, 25};
		int size = 5;
		
		int result = SumArray(numbers, size);
		printf("合計: %d\n", result);
	}
	```
	````

### ② コードの中の注目してほしい部分にコメントを書く
- コードブロックを使う場合、**コメントを使って意図や注目してほしい部分を明示する**と、回答の質を向上させることができる
- 問題が発生している行や、理解できない箇所に `// ここがわからない` などのコメントを追加する
- 実装したい機能や修正したい動作についても、コメントで具体的に説明すると効果的
- コメントは言語に合わせた形式で書く（C 言語の場合は `//`, Python の場合は `#` など）

#### 例

=== "🤔 コメントを活用しない"
	````txt title="プロンプト"
	次のコードの `IsEven` 関数の中身を完成させて。
	あと、2 行目のインクルードは何？

	```c
	#include <stdio.h>
	#include <stdbool.h>

	bool IsEven(int n)
	{

	}

	int main(void)
	{
		int n = 10;

		if (IsEven(n))
		{
			printf("%d は偶数です\n", n);
		}
		else
		{
			printf("%d は奇数です\n", n);
		}
	}
	```
	````

=== "✅ コメントを活用する"
	````txt title="プロンプト" hl_lines="5 7 10"
	次のコードの `IsEven` 関数の中身を完成させて。

	```c
	#include <stdio.h>
	#include <stdbool.h> // このインクルードは何？

	// 偶数の場合 true を返す
	bool IsEven(int n)
	{
		// ここがわからない
	}

	int main(void)
	{
		int n = 10;

		if (IsEven(n))
		{
			printf("%d は偶数です\n", n);
		}
		else
		{
			printf("%d は奇数です\n", n);
		}
	}
	```
	````


### ③ 警告やエラーメッセージを含める
- 発生した警告やエラーメッセージは、**コードブロック（言語指定なし）**でそのまま貼り付ける
- これにより、AI がメッセージの内容を正確に理解しやすくなる
- メッセージは**一部だけを抜き出さず、全文をそのままコピーする**

#### 例

=== "🤔 エラーメッセージを含まない"
	````txt title="プロンプト"
	このコードでエラーが発生した。原因と解決法は？

	```c
	#include <stdio.h>
	#include <math.h>

	int main(void)
	{
		double x;
		scanf("%lf", &x);
		printf("%f\n", sqrt(x));
	}
	```
	````

=== "🤔 エラーメッセージが不完全"
	````txt title="プロンプト"
	このコードでエラーが発生した。原因と解決法は？

	```c
	#include <stdio.h>
	#include <math.h>

	int main(void)
	{
		double x;
		scanf("%lf", &x);
		printf("%f\n", sqrt(x));
	}
	```

	```
	エラー: ld はステータス 1 で終了しました
	```
	````

=== "✅ エラーメッセージが完全"
	````txt title="プロンプト"
	このコードでエラーが発生した。原因と解決法は？

	```c
	#include <stdio.h>
	#include <math.h>

	int main(void)
	{
		double x;
		scanf("%lf", &x);
		printf("%f\n", sqrt(x));
	}
	```

	```
	/usr/bin/ld: /tmp/ccoLGRjM.o: in function `main':
	main.c:(.text+0x28): undefined reference to `sqrt'
	collect2: エラー: ld はステータス 1 で終了しました
	```
	````


## 5. C 言語の学習における活用例
C 言語の学習を進める上で、AI を使って次のような問題を解決することができる。ここでは有料モデルの回答例を示しているが、無料モデルでも基本的な質問には十分対応できる。ただし、回答の質や詳細度には差が生じる場合がある。

### ① 一般的な質問
````txt title="プロンプト"
私は理工学部の 1 年生です。
大学で C 言語を習うと何の役に立ちますか？
````

[ChatGPT-4o の回答 :material-open-in-new:](https://chatgpt.com/share/67dfae20-53f4-8009-8fb1-8fb81912bd46){:target="_blank" .md-button .md-button } [Claude 3.7 Sonnet の回答 :material-open-in-new:](https://claude.ai/share/4ea55f71-810d-49f0-ab18-f780b2526058){:target="_blank" .md-button .md-button }


### ② 学習上の悩みや気持ちの共有
````txt title="プロンプト"
大学の授業、C 言語や Linux のコマンドも覚えないといけないのに、
AI の使い方も覚えないといけないのは大変だー。
````

[ChatGPT-4o の回答 :material-open-in-new:](https://chatgpt.com/share/67dfdd4a-bf54-8009-ab0e-d1786af1ff82){:target="_blank" .md-button .md-button } [Claude 3.7 Sonnet の回答 :material-open-in-new:](https://claude.ai/share/83bac6e7-bff2-40ca-b1f0-8247d0250f9a){:target="_blank" .md-button .md-button }


### ③ 講義内容の疑問の解消
```txt title="プロンプト"
大学の C 言語の講義で Wandbox というサイトを紹介されたけど、これはどういうサイト？
なぜプログラムを実行できるの？
```

[ChatGPT-4o の回答 :material-open-in-new:](https://chatgpt.com/share/67dfae5a-50b8-8009-959c-b7f421c8f2f9){:target="_blank" .md-button .md-button } [Claude 3.7 Sonnet の回答 :material-open-in-new:](https://claude.ai/share/3335bcb7-d162-4f72-8865-097b32bdc63b){:target="_blank" .md-button .md-button }


### ④ エラーメッセージの解釈
````txt title="プロンプト"
このコードでエラーが発生した。原因と解決法は？

```c
#include <stdio.h>

int main(void)
{
	int n;
	scanf("%d", &n);

	int n;
	scanf("%d", &n);

	printf("%d\n", n + n);
}
```

```
main.c: 関数 ‘main’ 内:
main.c:8:13: エラー: リンク無し ‘n’ の再定義です
    8 |         int n;
      |             ^
main.c:5:13: 備考: previous declaration of ‘n’ with type ‘int’
    5 |         int n;
      |             ^
```
````

[ChatGPT-4o の回答 :material-open-in-new:](https://chatgpt.com/share/67dfae95-0a64-8009-a7fb-2e169f3d3eb8){:target="_blank" .md-button .md-button } [Claude 3.7 Sonnet の回答 :material-open-in-new:](https://claude.ai/share/7b739d96-6684-49da-89e1-da27bee61bfd){:target="_blank" .md-button .md-button }


### ⑤ コードの生成・補完
- AI は動作しないコードを生成することもあるため、回答は鵜呑みにせず、必ず自分でコンパイル・実行して確かめること

````txt title="プロンプト"
3 つの整数の最大値を返す関数を作成して。

```c
int Max(int a, int b, int c)
{

}
```
````

[ChatGPT-4o の回答 :material-open-in-new:](https://chatgpt.com/share/67dfaeca-75fc-8009-8e4e-3bc846621500){:target="_blank" .md-button .md-button } [Claude 3.7 Sonnet の回答 :material-open-in-new:](https://claude.ai/share/7de4d0c3-680d-4b35-8b8f-23a4f0f3ca7e){:target="_blank" .md-button .md-button }


### ⑥ 説明やドキュメントの作成
````txt title="プロンプト"
このプログラムを説明して。

```c
#include <stdio.h>

int main(void)
{
	int n;
	scanf("%d", &n);

	if (n == 2)
	{
		int a, b;
		scanf("%d%d", &a, &b);
		printf("%d\n", (a + b));
	}
	else if (n == 3)
	{
		int a, b, c;
		scanf("%d%d%d", &a, &b, &c);
		printf("%d\n", (a + b + c));
	}
}
```
````

[ChatGPT-4o の回答 :material-open-in-new:](https://chatgpt.com/share/67dfa92b-637c-8009-9ee5-ff8bb9522ae1){:target="_blank" .md-button .md-button } [Claude 3.7 Sonnet の回答 :material-open-in-new:](https://claude.ai/share/24a40ab0-6b52-483c-93f0-f2fbadf7a67b){:target="_blank" .md-button .md-button }


### ⑦ プログラムの改善
- 生成 AI は、厳格なエラーチェックや、特定のスタイルを積極的に推奨してくることがある
- 講義で扱っていない範囲のコードや、理解できないコードを AI が提案してきた場合は、無理に採用せず、まずはそのコードの意味を AI にたずねたり、教員や TA に相談したりすることを推奨する
- 必要に応じてプロンプトに次のような条件を追加し、過剰な修正を防ぐことができる

```
- 入力は必ず適切に行われるため、厳格なエラーチェックは不要。
- 関数の命名規則は PascalCase で統一する。
- C17 を想定。`main` 関数の冗長な return 0; は省略する。
- GCC でコンパイラ拡張を使わずにコンパイルできるようにする。
```

````txt title="プロンプト"
C 言語の練習で書いたプログラムです。改善できるところはある？

- 入力は必ず適切に行われるため、厳格なエラーチェックは不要。
- 関数の命名規則は PascalCase で統一する。
- C17 を想定。`main` 関数の冗長な return 0; は省略する。
- GCC でコンパイラ拡張を使わずにコンパイルできるようにする。

```c
#include <stdio.h>
#include <math.h>

double CircleArea(double r)
{
	return M_PI * pow(r, 2);
}

int main(void)
{
	double r;
	scanf("%lf", &r);
	printf("円の面積: %lf\n", CircleArea(r));
}
```
````

[ChatGPT-4o の回答 :material-open-in-new:](https://chatgpt.com/share/67dfa5fb-0148-8009-9bf4-af246a335696){:target="_blank" .md-button .md-button } [Claude 3.7 Sonnet の回答 :material-open-in-new:](https://claude.ai/share/0d3dd6cc-7fa5-46fc-a5b1-3090017b499a){:target="_blank" .md-button .md-button }


### ⑧ 自身の理解度確認
- 本講義では、講義資料を Markdown 形式のテキストファイルで別途配布する（Moodle）
- 利用する AI サービスがファイルアップロードに対応していれば、それを AI にアップロードすることで、講義内容に基づいた練習問題を作成してもらうことができる

````txt title="プロンプト"
この講義の内容を理解できたか確認したい。練習問題を作成して。模範解答を最後にまとめて。
````

## 6. 本講義の方針
- プログラミングは、人と AI の協働が最も進んでいる分野の 1 つ
- AI を活用して多くの人々が高速に学習を進めている時代に AI の利用を制限することは、学習機会の損失でもある
- AI を活用した問題解決プロセス（どのように質問し、得られた情報をどう活用したか）も評価したい
- 一方で、AI はあくまで学習を補助するツールであり、**利用は任意**。まずは自力で考え、必要に応じて AI を活用するというスタンスで問題ない。AI を使わずに課題を完成させても、もちろん満点を狙える
- **学習プロセスの評価**、**不正防止**、**TA・教員の適正なリソース分配**のために、次の 4 点を方針として設定する

### ① プロンプト履歴の記入義務
- [x] 提出課題を解く過程で AI と相談した場合、**課題解決に直接つながった主要な質問と回答を中心に、プロンプト履歴を提出に含める**
- プロンプト履歴は、議論の要約と URL をセットにして、提出課題の末尾に記入する 
- 共有 URL は、各 AI サービスのインターフェースにある『共有（Share）』ボタンなどから発行できることが多い。サービスでのアカウント登録が必要な場合がある
- 共有機能がない場合、主要なやり取り（自分の質問と AI の回答）をテキストでコピー & ペーストして添付する

````txt title="提出例"
#include <stdio.h>

int main(void)
{
	int a, b;
	scanf("%d %d", &a, &b);

	printf("%d\n", a + b);
}

//
// AI プロンプト履歴
//
// 1. 自分の書いたコードがコンパイルエラーになったため、AI に質問した
// https://chatgpt.com/share/67dfae95-0a64-8009-a7fb-2e169f3d3eb8
// 
// 2. より短く書く方法について質問した。また、"%d%d" と %d %d" の違いについても質問した
// https://chatgpt.com/share/67dfc39d-7440-8009-971e-fe57861ef636
//
````

- 異なる入力プロンプトに対して、**AI は完全に同じコードを生成することがある**
- そのため、ほとんどを AI に任せたコードをそのままコピペで提出すると「他者の提出と酷似」の判定を受けることがある
- プロンプト履歴を提出に含めることで、自身の作業過程を証明できる
- 実際、自分の力で書けるところまでコードを書き、自分の言葉で AI に質問し、その回答を自身で解釈して反映させれば、提出が他者と酷似することは起こらない（本講義ではそのような課題を設定する）


### ② AI とのコミュニケーションの評価
- [x] 提出課題が満点でなかった場合に、プロンプト履歴も採点対象とし、**100 点中 5 点を上限とする追加点**を与える
- 評価のポイント
	- 質問がこれまでの講義の理解に基づいているか、自身の努力が見られるか
		- すべてを AI に解決してもらうのではなく、自分の力で書いたコード、考えたことを最初に示しているか
		- まず自分で書けるところまで書いた形跡があるかを重視する
		- 例: `～という問題で ～ とういうコードを書いた。あとは ～ すればよいと思うが方法がわからない。`
	- AI の回答を鵜呑みにするだけのコミュニケーションになっていないか
		- 課題で求められていないコードを AI が提示した場合、適切に取捨選択しているか
		- AI が常に正しいとは限らないことを理解しているか
		- AI の回答を実際にコンパイル・実行して動作確認をしているか	
	- 自身の書いたコードや AI の書いたコードに対して深く説明できることを目指しているか
- 提出したプロンプトは、教員以外には公開されない
- 利用する AI の種類（無料 / 有料）によって評価が有利・不利になることはない

!!!note "プロンプトは完璧である必要はない"
	- 追加点は些少なので、無理にプロンプトを工夫して高得点を狙う必要はない
	- プロンプトの内容は、教員が学生の進度や理解度、疑問点を把握する目的でも使われる
	- 無理に高度な質問をすると、今後の口頭試問や提出課題の難度が上がり、成績評価に不利益をもたらす可能性がある
	- 実際のプロンプトを隠したり、取り繕ったりせず、正直な理解度や質問を示すことが望ましい


### ③ 質問はまず AI に
- [x] まずは AI に質問し、次のような場合に TA や教員に相談することを推奨する
	- AI が回答を提供できなかった場合
	- AI の回答が理解できなかった場合
	- AI の回答の妥当性を確認したい場合
	- 自分の理解と AI の回答にズレが生じていてモヤモヤする場合
	- 本学や本講義特有の事項について質問したい場合
- C 言語の初学者のつまずきや疑問の大半は AI が解決できる
- 人間に相談すると情報伝達に時間がかかったり、誤解を招いたりする可能性があるが、AI に相談することで、迅速に精度の高い回答を得られる
- Moodle の質問フォーラムに投稿する場合は、AI に質問した際のプロンプトの共有 URL を添付する
- TA や教員に直接質問する場合も、AI に質問した内容を共有し、その回答を踏まえた質問をすることで、より効果的なコミュニケーションが可能になる


### ④ 注意点
- 自分や他人の個人情報、所属組織の機密情報などをプロンプトに入力しないこと
- AI 利用を禁止している講義では、その講義のルールに従うこと
- 本講義では、口頭試問と筆記試験では AI を利用できない

## 7. このページについて
- このページは、[**Ryo Suzuki** :material-open-in-new:](https://x.com/Reputeless){:target="_blank"} が、早稲田大学で担当する C プログラミング入門講義のために作成した AI 利用ガイドを、外部公開用に改変したものです
- ページのソースを Markdown 形式で [GitHub にて公開 :material-open-in-new:](https://github.com/Reputeless/using-ai){:target="_blank"}しています（ライセンス CC0）
- 自由に改変して活用してください

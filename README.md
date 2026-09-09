# research_oee

## このリポジトリについて

このリポジトリは、**Open-Ended Evolution（OEE）の理論・証拠・方法論研究を整理した研究リポジトリ**です。中心的な問いは次のとおりです。

$$
\boxed{
\text{なぜ人工進化系は収束・閉鎖しやすいのに、}
\atop
\text{自然進化は新しい進化可能性を生成し続けているように見えるのか？}
}
$$

現在、この問いを説明する一般的な mechanism は確立していません。このリポジトリは implementation phase ではなく、理論候補を既存研究と反例に照らして検査した後、hallmark ごとの証拠と方法論を整理し、**empirical exemplar boundary で pause** しています。

この README は、初めて訪れた人が「何の研究か」「どの文書を何のために読むか」を判断するための **navigation / orientation layer** です。canonical research state、frontier、hypothesis、next operation の出典ではありません。

## 現在の研究状態

2026年9月時点の canonical conclusion は次のとおりです。

- literature / methodology phase は完了
- heterogeneous empirical boundary に到達
- AFN program は外部独立検証待ちで paused
- complexity program は strong-S / strong-I conjunction exemplar 待ちで paused
- exemplar program は empirical boundary に到達
- mechanism research は未準備
- implementation は正当化されていない

研究全体の exact next operation は **GLOBAL PAUSE — EMPIRICAL EXEMPLAR BOUNDARY** です。これは OEE が説明済み、あるいは分野全体が尽きたという意味ではありません。

> 最新状態は必ず [STATUS.md](STATUS.md) を参照してください。

## 最初に読む

正式な入口は、次の優先順です。

### 1. [STATUS.md](STATUS.md)

現在地を最短で確認する文書です。現在の研究状態、主要な確定事項、pause / blocked 状態、mechanism readiness、exact next operation と unblock condition を圧縮しています。研究を再開するときは、まずここを読んでください。

### 2. [FRONTIER.md](FRONTIER.md)

未解決問題と停止理由を確認する文書です。`ACTIVE`、`PAUSED`、`BLOCKED`、`CLOSED` などの frontier 状態と、各 branch を再開できる条件を記録しています。「何がまだ問題なのか」を確認したいときに読みます。

### 3. [KNOWN.md](KNOWN.md)

研究中に確定した durable conclusions、再び調べる必要のない境界、terminology / evidence distinctions を収めた安定知識の canonical record です。「このリポジトリが既に何を知っているか」を確認するときに読みます。

### 4. [AGENTS.md](AGENTS.md)

研究エージェントの行動規則です。research workflow、hypothesis firewall、one-pass rule、repository maintenance、closed frontier を別の用語で再開しない規則を定めています。Codex / AI agent を再び研究に使う場合は必読です。

### 5. [HYPOTHESES.md](HYPOTHESES.md)

仮説として昇格した内容を置く canonical file です。現在は空ですが、未完成だからではありません。最終判断が次であるためです。

$$
\boxed{
\text{HYPOTHESIS GENERATION PREMATURE FOR EMPIRICAL REASONS}
}
$$

## 二つの読み方

### A. 研究を再開したい

次の順に読みます。

1. `STATUS.md`
2. `FRONTIER.md`
3. `KNOWN.md`
4. `AGENTS.md`
5. 再開条件に関係する synthesis / methodology artifact

この用途では、`docs/archive/RESEARCH_RETROSPECTIVE_JA.md` を research state や next-action source として使用しないでください。

### B. この研究が何をしてきたのか振り返りたい

最初に [RESEARCH_RETROSPECTIVE_JA.md](docs/archive/RESEARCH_RETROSPECTIVE_JA.md) を読みます。

> 注意: この文書は人間向けの振り返りであり、research state の canonical source ではありません。AI agent の next-action decision には使用しません。

これは **NON-NORMATIVE RETROSPECTIVE ARCHIVE** です。研究開始時の問題意識、思考の変化、棄却した方向、AFN、complexity、exemplar program、最終 pause を日本語で振り返るための human-readable document です。将来の研究判断では canonical files を優先してください。

## 目的別の読み方

### 5分で現在地を把握

1. `STATUS.md`
2. `FRONTIER.md`
3. [SYNTHESIS_008_GLOBAL_OEE_RESEARCH_BOUNDARY.md](SYNTHESIS_008_GLOBAL_OEE_RESEARCH_BOUNDARY.md)

### 研究全体を日本語で振り返る

1. `docs/archive/RESEARCH_RETROSPECTIVE_JA.md`
2. 必要に応じて `SYNTHESIS_008_GLOBAL_OEE_RESEARCH_BOUNDARY.md`

archive は振り返り専用であり、最新の研究判断には canonical files を用います。

### 理論研究の流れを追う

1. [SYNTHESIS_001_Q001_Q012.md](SYNTHESIS_001_Q001_Q012.md)
2. [SYNTHESIS_002_Q013_Q021.md](SYNTHESIS_002_Q013_Q021.md)
3. [SYNTHESIS_003_Q022_Q027.md](SYNTHESIS_003_Q022_Q027.md)

### AFN を追う

`EVIDENCE_MATRIX_001` → `METHODOLOGY_001` / `APPLICATION_001` / `FORMALIZATION_001` / `METHODOLOGY_002` → `VALIDATION_001` / `ANALYSIS_001` / `VALIDATION_002` → `SYNTHESIS_004` の順に、evidence、methodology、validation、program consolidation を追います。

### Complexity を追う

`EVIDENCE_MATRIX_002` → `METHODOLOGY_003` → `APPLICATION_002` → `EVIDENCE_MAP_003` → `SYNTHESIS_006` の順に読みます。

### Exemplar 問題を追う

`SYNTHESIS_007` → `EVIDENCE_MATRIX_004` → `SPECIFICATION_001` → `VALIDATION_003` → `SYNTHESIS_008` の順に読みます。

## ドキュメント構成

### Canonical state

以下が canonical layer です。

| 文書 | 役割 |
| --- | --- |
| `STATUS.md` | 現在の研究状態、readiness、next operation、unblock condition |
| `FRONTIER.md` | 未解決・停止・閉鎖された frontier |
| `KNOWN.md` | 安定した研究知識と確定済みの境界 |
| `HYPOTHESES.md` | hypothesis firewall を通過して昇格した仮説 |
| `AGENTS.md` | AI agent / Codex の研究規則 |

research-state authority の precedence は次のとおりです。

$$
\boxed{
\texttt{AGENTS.md + STATUS.md + FRONTIER.md + KNOWN.md + HYPOTHESES.md}
>
\texttt{README.md}
>
\texttt{docs/archive/RESEARCH\_RETROSPECTIVE\_JA.md}
}
$$

ここで `>` は科学的重要性の順位ではなく、**research-state authority** の優先順位を表します。

### Theoretical synthesis

`SYNTHESIS_*` は、各 research phase の経路・棄却・残存境界を圧縮した checkpoint です。現在状態そのものは `STATUS.md` を優先してください。

- [SYNTHESIS_001_Q001_Q012.md](SYNTHESIS_001_Q001_Q012.md): 初期 theoretical decomposition。closure、observer / latent capacity、function、generative capacity、accessibility、transition propensity を分離します。
- [SYNTHESIS_002_Q013_Q021.md](SYNTHESIS_002_Q013_Q021.md): organizational change、individuality、reproduction / heredity と evidence / instrumentation boundary を整理します。
- [SYNTHESIS_003_Q022_Q027.md](SYNTHESIS_003_Q022_Q027.md): 初期 mechanism-space decomposition の終端です。判断は **current repository decomposition exhausted** であり、field exhaustion ではありません。ここから hallmark-first / evidence-first へ移行しました。
- [SYNTHESIS_004_AFN_HALLMARK_PROGRAM.md](SYNTHESIS_004_AFN_HALLMARK_PROGRAM.md): Adaptive Functional Novelty program の consolidation。AFN method phase は完了し、external independent validation boundary で pause しています。
- [SYNTHESIS_005_NEXT_OEE_HALLMARK.md](SYNTHESIS_005_NEXT_OEE_HALLMARK.md): AFN 後の hallmark selection。ongoing evolutionary growth of nontrivial complexity を次の target に選びました。
- [SYNTHESIS_006_COMPLEXITY_HALLMARK_PROGRAM.md](SYNTHESIS_006_COMPLEXITY_HALLMARK_PROGRAM.md): complexity program の consolidation。strong-S / strong-I conjunction exemplar が reviewed search space に存在しないという境界を確定しました。
- [SYNTHESIS_007_GLOBAL_OEE_EXEMPLAR_GAP.md](SYNTHESIS_007_GLOBAL_OEE_EXEMPLAR_GAP.md): component exemplars は存在するが、broad artificial-OEE exemplar は確立していないという global exemplar problem を整理します。
- `SYNTHESIS_008_GLOBAL_OEE_RESEARCH_BOUNDARY.md`: 現在の最終 global checkpoint で、この repository state を理解するうえで最重要の synthesis です。中心結果は **GLOBAL LITERATURE/METHODOLOGY PHASE COMPLETE, EMPIRICAL BOUNDARY REACHED** です。

#### Q-series / theoretical research

Q001–Q027 系は、魅力的な mechanism candidate を既存理論、prior art、counterexample に照らして破壊的に検査した理論経路です。

$$
\boxed{
\text{mechanism candidate}
\rightarrow
\text{prior art / counterexample による destructive test}
}
$$

全 Q-note を入口から読む必要はありません。詳細な理論経路や特定 branch の棄却理由を追う場合に、対応する synthesis から個別の Q-document へ進んでください。なお、repository に `Q001` note はなく、その surviving results は `KNOWN.md` の K001–K007 に保存されています。

### Adaptive Functional Novelty

AFN は、適応的で、遺伝し、既存とは異なる機能クラスの新規性を、同一の event-history 上で評価する hallmark program です。中心的な evidence structure は次です。

$$
\boxed{N\land F\land H\land A\land C}
$$

- `N`: novelty
- `F`: function
- `H`: heredity
- `A`: adaptive consequence
- `C`: functional-class distinctness

#### AFN evidence

- [EVIDENCE_MATRIX_001_ADAPTIVE_FUNCTIONAL_NOVELTY.md](EVIDENCE_MATRIX_001_ADAPTIVE_FUNCTIONAL_NOVELTY.md): 複数の人工進化 system について、AFN の各証拠リンクと heterogeneous bottleneck を比較した evidence map です。
- [VALIDATION_001_STRINGMOL_ADAPTIVE_FUNCTIONAL_NOVELTY.md](VALIDATION_001_STRINGMOL_ADAPTIVE_FUNCTIONAL_NOVELTY.md): Stringmol における有限回の反復 AFN を検証し、同一 history 内で二つの ordered event を支持します。
- [ANALYSIS_001_STRINGMOL_STATIC_HISTORY_REANALYSIS.md](ANALYSIS_001_STRINGMOL_STATIC_HISTORY_REANALYSIS.md): deposited Stringmol history に対する read-only static analysis です。simulation や Stringmol executable を再実行せず、既存の processed histories を検査しました。
- [VALIDATION_002_AVIDA_GEB_ADAPTIVE_FUNCTIONAL_NOVELTY.md](VALIDATION_002_AVIDA_GEB_ADAPTIVE_FUNCTIONAL_NOVELTY.md): Avida / Geb と比較し、Stringmol が strongest finite repeated-AFN case のままであることを確認しました。これは ongoing AFN の確立ではありません。

#### AFN methodology

- [METHODOLOGY_001_AFN_EVENT_HISTORY.md](METHODOLOGY_001_AFN_EVENT_HISTORY.md): AFN event-history methodology。中心は `detection → reconstruction → validation` で、N/F/H/A/C、provenance、deduplication、censoring を一つの workflow に統合します。
- [APPLICATION_001_AFN_EVENT_HISTORY_CROSS_SYSTEM.md](APPLICATION_001_AFN_EVENT_HISTORY_CROSS_SYSTEM.md): frozen methodology を Stringmol / Avida / Geb に retrospective cross-system application した文書です。
- [FORMALIZATION_001_AFN_FUNCTIONAL_CLASS_IDENTITY.md](FORMALIZATION_001_AFN_FUNCTIONAL_CLASS_IDENTITY.md): functional class を `SAME / DISTINCT / UNRESOLVED` で判定します。中心的な区別は `activity → causal role → adaptive consequence` です。
- [METHODOLOGY_002_AFN_INDEPENDENT_CODING_ROBUSTNESS.md](METHODOLOGY_002_AFN_INDEPENDENT_CODING_ROBUSTNESS.md): independent coding / analyst robustness の protocol です。AFN が最終的に止まった **external independent validation** boundary を理解する文書です。

### Complexity Growth

この program は、観測された複雑性増加と、資源を増やしたときの到達可能 frontier の拡張を分離します。

$$
\boxed{
\text{realized complexity growth}
\neq
\text{resource-scalable complexity frontier}
}
$$

repository では、$S$ を **sustained realized complexity evidence**、$I$ を **resource-scalability evidence** として扱います。

#### Complexity evidence

- [EVIDENCE_MATRIX_002_COMPLEXITY_GROWTH.md](EVIDENCE_MATRIX_002_COMPLEXITY_GROWTH.md): Avida、Geb、Tierra、Stringmol、Flow-Lenia などの cross-system evidence map です。complexity object、realized growth、scalability、triviality control を分けて比較します。
- [EVIDENCE_MAP_003_COMPLEXITY_STRONG_S_STRONG_I_SEARCH.md](EVIDENCE_MAP_003_COMPLEXITY_STRONG_S_STRONG_I_SEARCH.md): expanded positive-case search。主要結果は Aevol `(S2,I0)`、Geb `(S1,I4)` で、strong S / strong I conjunction case は見つかりませんでした。

#### Complexity methodology

- [METHODOLOGY_003_COMPLEXITY_SUSTAINEDNESS_SCALABILITY.md](METHODOLOGY_003_COMPLEXITY_SUSTAINEDNESS_SCALABILITY.md): $S$ と $I$ を分離し、同じ defensible complexity object に対する temporal sustainedness と resource scalability を評価する methodology です。
- [APPLICATION_002_COMPLEXITY_SUSTAINEDNESS_SCALABILITY_CROSS_SYSTEM.md](APPLICATION_002_COMPLEXITY_SUSTAINEDNESS_SCALABILITY_CROSS_SYSTEM.md): frozen methodology を複数 system に適用した retrospective validation です。

### OEE Exemplars

Bedau 2024 の exemplar problem と整合する範囲で、この repository は次を区別します。

$$
\boxed{\text{component scientific exemplars exist}}
$$

$$
\boxed{\text{broad artificial-OEE exemplar not established}}
$$

ここで exemplar は、単なる有名な model 名ではなく、特定の科学的問題に対する **model + measure + interpreted result** の package です。

- [EVIDENCE_MATRIX_004_OEE_CANDIDATE_EXEMPLARS.md](EVIDENCE_MATRIX_004_OEE_CANDIDATE_EXEMPLARS.md): Evoloops、Stringmol、Avida、Aevol、Geb、Genelife、Flow-Lenia、Outlier を `model + measure + result` として比較します。「どの system が一番 OEE か」という scalar ranking ではなく、各 package が何を legitimately exemplify するかを示す partial comparison です。

### Evidence Specification

- [SPECIFICATION_001_PROSPECTIVE_OEE_EXEMPLAR_EVIDENCE.md](SPECIFICATION_001_PROSPECTIVE_OEE_EXEMPLAR_EVIDENCE.md): 将来の artificial-OEE candidate study が claim を audit 可能にするために残すべき evidence と provenance の guidance です。次の三つを分けます。

$$
\boxed{
\text{reproducibility}
\neq
\text{claim auditability}
\neq
\text{exemplar status}
}
$$

これは community standard ではなく、repository guidance です。

- [VALIDATION_003_PROSPECTIVE_OEE_SPEC_RETROSPECTIVE_AUDIT.md](VALIDATION_003_PROSPECTIVE_OEE_SPEC_RETROSPECTIVE_AUDIT.md): Specification 001 を既存 exemplars に逆適用しました。結果は **validated with minor refinement needs**、low bureaucratic overhead、zero logical substrate exceptions であり、specification は **retrospectively validated as repository guidance** と判定されています。これは broad exemplar の成立を意味しません。

### Human Retrospective Archive

#### 人間向け振り返り

[RESEARCH_RETROSPECTIVE_JA.md](docs/archive/RESEARCH_RETROSPECTIVE_JA.md) は、日本語で conceptual history、research decisions、rejected directions、AFN、complexity、exemplar program、pause の意味をたどる文書です。

$$
\boxed{\text{NON-NORMATIVE}}
$$

研究再開時の state source ではありません。内容が canonical state と競合する場合は、canonical files を優先します。

## 重要な研究上の区別

この repository では、少なくとも次を同一視しません。詳細な定義と根拠は `KNOWN.md` および各 artifact を参照してください。

$$
\text{continued evolution}\not\Rightarrow\text{OEE}
$$

$$
\text{observed novelty absence}
\neq
\text{novelty capacity absence}
$$

$$
\text{formal constructibility}
\neq
\text{evolutionary accessibility}
$$

$$
\text{Darwinian evolution}\not\Rightarrow\text{OEE}
$$

$$
\text{finite AFN}\neq\text{ongoing AFN}
$$

$$
\text{complexity growth}\neq\text{resource scalability}
$$

$$
\text{component exemplar}\neq\text{broad OEE exemplar}
$$

### 最低限の用語

- **OEE**: Open-Ended Evolution。単なる継続的変化や多様性ではなく、新しい進化可能性が持続的に生成されるという問題領域。
- **AFN**: Adaptive Functional Novelty。新規性、機能、遺伝、適応的帰結、機能クラスの差異を分離して評価する hallmark。
- **S / I**: realized complexity の時間的 sustainedness と、資源拡張に対する frontier scalability の証拠クラス。
- **exemplar**: 特定の問題に対する再利用可能な model–measure–result package。broad OEE の証明とは限りません。
- **canonical state**: 現在の判断を権威的に保持する `STATUS.md`、`FRONTIER.md`、`KNOWN.md`、`HYPOTHESES.md` と、それらの運用規則を定める `AGENTS.md`。

## HYPOTHESES.md が空である理由

現在の空状態は deliberate research state です。

$$
\boxed{
\text{hypothesis generation premature for empirical reasons}
}
$$

AFN、complexity、exemplar の検討によって証拠境界は明確になりましたが、stable positive phenomenon、credible positive exemplar、matched negative / interventional contrast、causal discriminability の組合せが不足しています。そのため、mechanistic hypothesis を昇格させる段階ではありません。

また、次の方向は既に destructive analysis 済みであり、単に新しい名称を付けて未研究テーマとして再開しません。

- universal transition mechanism
- unconditional broad-scope evolvability
- organizational-type creation
- generic ecological selection-structure mechanism
- universal continuity invariant

closed / decomposed / blocked の正確な範囲は `KNOWN.md` と `FRONTIER.md` を確認してください。

## なぜ実装コードが中心ではないのか

このリポジトリは software project というより、**research reasoning / evidence repository** です。

- artificial-life system の implementation 自体は目的ではありません。
- mechanism justification より前に system や architecture を実装しません。
- 文献、証拠、反例、測定条件、falsification boundary を研究記憶として保存します。
- 例外的に、deposited Stringmol history の read-only static analysis のような限定的 computational analysis は存在しますが、新しい simulation の実行ではありません。

## AI agent / Codex で研究を再開する場合

現在は **GLOBAL PAUSE** 中です。再開条件を満たす新しい empirical resource がない限り、研究 task を作ること自体を進歩と見なしません。

1. `README.md` は navigation document にすぎません。
2. `docs/archive/RESEARCH_RETROSPECTIVE_JA.md` は retrospective only です。
3. 必ず `AGENTS.md` を読み、research workflow と禁止事項に従います。
4. `STATUS.md` で現在状態、mechanism readiness、exact next operation を確認します。
5. `FRONTIER.md` で active / paused / blocked / closed と unblock condition を確認します。
6. `KNOWN.md` で closed knowledge と既に確定した区別を確認します。
7. closed branch を新しい terminology で再開しません。
8. `HYPOTHESES.md` を根拠なく埋めません。

再開するときも、条件が満たされた branch だけを最小の research scale で扱います。

## このリポジトリでの「完了」と「停止」

$$
\boxed{\text{pause}\neq\text{failure}}
$$

現在停止している理由は、内部の literature / methodology work をさらに増やすより、新しい empirical evidence、外部独立検証、same-object history、または matched causal contrast の情報価値が高くなったためです。

$$
\boxed{
\text{new empirical evidence の価値}
>
\text{追加の internal literature / methodology work の価値}
}
$$

「何か次の task を作ること」を進歩とはみなしません。停止条件を守り、unblock condition が満たされるまで pause を維持することも、premature mechanism や implementation を防ぐ研究成果の一部です。

## ライセンス / 引用

本リポジトリには、この README 作成時点で明示的なライセンス情報がありません。引用・出典については、各 research artifact の references を参照してください。

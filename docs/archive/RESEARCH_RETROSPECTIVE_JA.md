# OEE 理論研究の振り返り

> **NON-NORMATIVE RETROSPECTIVE ARCHIVE — 非規範的な回顧アーカイブ**
>
> この文書は、研究活動を人間が振り返るための非規範的なアーカイブである。
>
> `STATUS.md`、`FRONTIER.md`、`KNOWN.md`、`AGENTS.md` の代替ではない。
>
> 将来の研究エージェントは、この文書を現在状態、未解決 frontier、次の行動、仮説生成の根拠として使用してはならない。
>
> 現在の研究状態を確認するときは canonical files を参照すること。

この文書は、2026年9月までにこの repository で行った研究を、数か月後、あるいは数年後の人間の自分が読み返すために書いたものである。目的は結果の一覧化ではない。なぜ問いを立て、どの説明に惹かれ、何を区別できていなかったのか、どの時点で研究の進歩の意味が変わり、なぜ最後に止まったのかを再構成することにある。

以下では、既存 artifact が確定した内容を **事実**、それらを研究史としてまとめ直した記述を **解釈** と呼ぶ。この文書は新しい仮説、予測、研究計画を含まない。

## 1. 出発点――なぜこの研究を始めたのか

研究開始時の中心には、単純だが重い問いがあった。

$$
\boxed{
\text{なぜ人工進化系は収束・閉鎖しやすいのに、}
\atop
\text{自然進化は新しい進化可能性を生成し続けているように見えるのか？}
}
$$

**事実。** 出発点には Evoloops、Lenia / Flow-Lenia、Autopoiesis、Open-Ended Evolution（OEE）、そして modern deep learning から得られる抽象的な構造上の示唆があった。Evoloops は局所規則のもとで自己複製、遺伝的変異、内在的選択、適応が成立する最小限の基準例だった。Lenia と Flow-Lenia は連続的で変形可能な形態、物質流、境界の曖昧さを含む基質の候補だった。Autopoiesis は自己維持、組織的閉包、個体にとっての意味や機能を考える手掛かりだった。deep learning は、表現力と実際の到達可能性、表現の変化、構成性、学習可能性を区別する比喩を与えた。

**当時の期待。** これらを合わせれば、固定された離散的複製子よりも、自己を維持しながら形態と関係を変え、新しい進化の自由度を開く system concept に近づけるように見えた。粗い形では、関心は次の和として表せた。

$$
\text{Evoloops}
+
\text{Lenia}
+
\text{Autopoiesis}
+
\text{OEE}
$$

しかし、この魅力は科学的説明ではなかった。自己複製、連続形態、自己維持、豊かなダイナミクスは、それぞれ重要であっても、それらを並べるだけでは「なぜ進化可能性が更新され続けるのか」という因果問題に答えない。deep learning の仕組みも人工生命へ直接移植できるものではなく、進化学にすでに存在する概念を別名で持ち込む危険があった。

## 2. 最初の大きな転換――system building から理論境界へ

研究の最初の大きな転換は、魅力的な system を考えることと、OEE の mechanism を理解することを分離した点にあった。

$$
\boxed{
\text{魅力的な構成要素を組み合わせること}
\neq
\text{OEE mechanism を理解すること}
}
$$

**解釈。** 初期の統合案には、問いを具体化する価値があった。だが、構成要素を増やすほど、どの要素が何を説明したのかは逆に分からなくなる。仮に Evoloops–Lenia–autopoiesis hybrid が豊かな挙動を示しても、それが replication、morphological diversity、adaptive novelty、complexity、あるいは OEE のどれなのかを識別できなければ、system-building の成功と理論的成功は一致しない。

そこで方針は、「まず作ってから意味を考える」方向ではなく、実装より前に既知理論と証拠の境界を確定する方向へ移った。中心に置かれたのは、次の区別だった。

$$
\text{known evidence}
\rightarrow
\text{abstraction}
\rightarrow
\text{research frontier}
\rightarrow
\text{falsifiable hypothesis}
$$

この順序は、実装を永久に拒む原則ではない。何を実装すれば競合説明を識別できるのかが決まるまで、実装を科学的前進と取り違えないための順序だった。

## 3. Q001–Q027 で実際に潰していったもの

Q001–Q027 は27個の発見を直列に積んだ記録ではない。より正確には、OEE を説明しているように見える言葉の間に境界線を引き、説明候補を prior art、定義問題、測定問題、あるいは empirical blockage へ戻していく過程だった。

### 3.1 replication / evolution は OEE ではない

**事実。** Evoloops は自己複製、遺伝的変異、差次的繁殖、適応を示す。しかし、それだけでは持続的な OEE を示さない。ある observable の plateau も、将来の可能性が閉じたことの証明ではない。

$$
\text{replication}
\not\Rightarrow
\text{Darwinian evolution}
\not\Rightarrow
\text{OEE}
$$

ここで重要だったのは、途中の含意を一つずつ検査することだった。複製があっても heritable variation がなければ進化ではない。進化があっても adaptive novelty が続くとは限らない。多様性、活動、複雑性の増加も、それぞれ OEE とは別の主張である。

### 3.2 observed novelty と latent capacity は違う

**事実。** 有限の観察窓で新しいものが現れなかったことは、到達不能性を意味しない。逆に、論理的に構成可能であることも、進化が現実的な時間と資源のもとで到達できることを意味しない。

$$
\text{non-observation}
\neq
\text{inaccessibility},
\qquad
\text{formal possibility}
\neq
\text{evolutionary accessibility}
$$

到達可能性は、経路の存在だけでなく、経路の多さ、到達確率、待ち時間、途中状態の viability、遺伝、集団内での establishment、資源負担を含む分布的な問題だった。大きな state space は大きな「有効な進化可能性空間」ではない。

### 3.3 new dependency と new function は違う

**事実。** 新しい依存関係、自己維持への寄与、selected effect、causal role、将来の能力は同一ではない。constructive neutral evolution や entrenchment は、組織や依存が増えても新しい適応機能や将来の生成能力が増えない反例を与えた。

Autopoiesis は、誰にとって何が維持されるのかを domain-specific に基礎づけるうえで有用だった。しかし organizational closure は evolutionary closure の反対語ではなく、自己維持は新しい遺伝的機能の継続的生成を保証しない。

### 3.4 formal constructibility と evolutionary accessibility は違う

**事実。** universal constructor、万能な表現言語、拡張可能な substrate、自己参照規則は、原理的な構成能力を与え得る。しかし、それらは evolutionary search が有効な経路を発見し、維持し、次の革新へつなげることを保証しない。

$$
\text{constructible}
\not\Rightarrow
\text{discoverable}
\not\Rightarrow
\text{established}
\not\Rightarrow
\text{recurrently generative}
$$

この区別は deep learning から得た「expressivity と trainability は違う」という直観と響き合ったが、研究上の中身は genotype–phenotype map、evolvability、neutral network、first-passage、scalable evolvability といった既存の進化理論に吸収された。

### 3.5 mechanism change と identity change は違う

**事実。** 実装や因果配線が大きく変わっても同じ character や reproductive life cycle と見なせる場合があり、小さな変化が新しい reproduction relation を成立させる場合もある。causal abstraction は、選んだ不変量が保たれるかを検査できるが、何を identity-bearing relation とすべきかを自動的には決めない。

Q013–Q021 で「endogenous organizational type」という一般名は、morphological novelty、collective reproduction、collective heredity、Darwinian individuality、autonomy、character identity へ分解された。Snowflake yeast と Fernandes の比較から得られた重要な教訓は、frozen criterion の transfer failure が、そのまま存在論的な非同一性を意味しないことだった。clonality、fragmentation、propagule size は特定系での realizer であり、一般的な collective reproduction の必要条件ではない。

Fernandes については、理論的 criterion が欠けていたのではない。collective heredity を判定するには、独立に割り当てられた parentage、親間変異、同環境の非親を超える親特異的予測、子が次に繁殖する concatenated edge が必要だった。しかし published output には、それを決める event-complete pedigree がなかった。ここで残ったのは theoretical gap ではなく instrumentation gap だった。

### 3.6 major transition の存在と recurrent transition mechanism は違う

**事実。** major transition は reproduction、heredity、individuality、selection の単位を変え得る。複数の transition が歴史上存在することも確かである。しかし、有限個の transition の列は、それらを繰り返し生成する一つの mechanism の存在を含意しない。

$$
\text{repeated transitions}
\neq
\text{a recurrence mechanism}
$$

各 transition は ecological scaffolding、conflict mediation、life-cycle closure、endogenization、historical contingency など異なる局所原因で説明できる。ある transition が次を促進することも抑制することもあり、組織化は可能性を単調に増やす ladder ではない。単位が変わっても、continuity は一つの bearer の保存ではなく、ancestry、reproduction、reconstruction、life cycle、selected contribution など domain-specific な関係によって記述できた。

### 3.7 evolvability に universal unconditional solution はない

**事実。** robustness、modularity、cryptic variation、potentiation、modifier、developmental organization は、宣言された条件のもとで将来の適応へのアクセスを改善し得る。しかし、任意の未知の将来課題へ無条件に generalize する evolvability は、共有構造、対応関係、現在の効用、反復性、あるいは遺伝的関連なしには選択され得ない。

$$
\text{evolvability gain under conditions}
\neq
\text{universal preparedness for arbitrary futures}
$$

この no-free-lunch boundary によって、modern deep learning の generalization や meta-learning を、そのまま OEE mechanism として移植する道は閉じた。

### 3.8 fixed microphysics と fixed evolutionary organization は違う

**事実。** 物理法則や局所 microdynamics が固定されていても、regulation、development、inheritance channel、selectable unit といった effective evolutionary organization は変化し得る。したがって、OEE を説明するために literal な物理 state space の拡張を要求する必要はない。

しかし逆向きも重要だった。effective organization が一度変わることは、そのような変化が継続的に起こることを意味しない。暫定表現

$$
\mathcal S_t=(X_t,\mathcal O_t),
\qquad
\mathcal O_t=(V_t,R_t,H_t,S_t)
$$

や

$$
(X_t,\mathcal O_t)\rightarrow(X_{t+1},\mathcal O_{t+1})
$$

は、考えるべき差を可視化したが、それ自体は mechanism でも、OEE の確立した定義でもなかった。adjacent possible、evolving genotype–phenotype maps、evolution of evolvability、major transitions などがすでに近い内容を扱っていた。

### 3.9 多くの mechanism 候補が「発見」にならなかった理由

**解釈。** この段階の最大の成果は、新しい名前を増やさなかったことにある。「generative capacity」「organizational-type creation」「new selection structure」「self-maintaining plasticity」「transition propensity」といった候補は、攻撃すると、既存理論の再命名、複数既知機構の単純な conjunction、domain-specific な定義問題、測定問題、または unavailable data に分解された。

$$
\boxed{
\text{多くの「新しい mechanism 候補」が}
\atop
\text{既存理論・定義・measurement problem に吸収された}
}
$$

これは研究が空振りしたという意味ではない。誤って独創性を主張し得た場所に、prior-art boundary と inference firewall が置かれたという意味である。

## 4. `NO HYPOTHESIS JUSTIFIED` は何を意味したか

研究中、何度も `NO HYPOTHESIS JUSTIFIED` という結論になった。

**事実。** アイデアがなかったわけではない。むしろ候補は多かった。生態的 feedback、self-reference、autopoietic closure、recursive transitions、evolution of evolvability、substrate richness、compositionality、resource scaling、coupled nonstationarity など、説明になりそうな方向は繰り返し現れた。

**解釈。** それらを仮説へ昇格させる前に、すでに知られた概念ではないか、反例があるか、対象 hallmark が安定しているか、positive/negative contrast があるか、何が falsify するかを破壊的に検査した。その結果が空集合だった。

$$
\boxed{
\text{魅力的な説明候補を}
\atop
\text{仮説へ昇格させる前に破壊的に検査した}
}
$$

したがって `NO HYPOTHESIS JUSTIFIED` は、LLM の失敗でもテーマの無意味さでもない。仮説ファイルを埋めることより、根拠の弱い仮説を通さないことを優先した記録である。

## 5. SYNTHESIS 003――mechanism-first から hallmark-first へ

Q022–Q027 の終了時、repository は次の判断に達した。

$$
\boxed{
\text{repository's current decomposition of OEE mechanism space exhausted}
}
$$

**事実。** F1–F5 と cross-unit continuity は、現在の定式化のもとでは closed、decomposed、または empirically blocked になった。だが、これは次を意味しなかった。

$$
\boxed{
\text{OEE field exhausted}
}
$$

OEE literature は adaptive novelty、complexity growth、evolving evolvability、major transitions、semantic evolution、exploratory / expansive / transformational novelty など、非同値な behavioral hallmarks を含んでいた。repository の探索は transition、unit、identity、heredity に深く寄り、当初の不満に近い「新しい適応的な生き方が続けて現れる」という現象そのものを、直接比較していなかった。

**解釈。** ここで研究戦略は mechanism-first から次へ変わった。

$$
\boxed{
\text{hallmark-first / evidence-first}
}
$$

原因を考える前に、まず何が起きたときに対象現象を認めるのか、既存 system のどの history がその証拠を持つのかを確定する。この転換によって、次の研究段階は mechanism の命名ではなく、Adaptive Functional Novelty（AFN）の evidence decomposition になった。

## 6. AFN program――新しい機能を「出来事」として読む

### 6.1 AFN を選んだ理由

AFN program が問うたのは、単なる新しい configuration や genotype ではなく、系の持続や繁殖に新しい causal contribution を与えるものが、歴史の中で生まれ、遺伝し、適応的に成立し、異なる機能 class として繰り返し現れたかだった。

中心の evidence chain は次である。

$$
\boxed{N\land F\land H\land A\land C}
$$

- **N — historical novelty:** 宣言された観察 history と resolution において、それ以前に同等の役割が確認されない。
- **F — function:** system-grounded な causal role がある。
- **H — heredity / reconstruction:** その役割を担う組織が、選択が働ける程度に伝達・再構成される。
- **A — adaptation:** 比較または lineage evidence により、繁殖成功や適応的持続への寄与が支持される。
- **C — class distinctness:** 既知 event の単なる実装変更や改良ではなく、宣言した比較契約のもとで異なる causal role である。

**事実。** どれか一つだけでは AFN にならない。活動していることは function の証拠ではなく、持続は heredity や adaptation の証拠ではなく、fitness の違いは function class の identity を定義しない。

### 6.2 Stringmol が重要になった理由

Stringmol は、単に artificial chemistry として面白かったのではない。長い連続 history と reaction semantics が残り、異なる時点の event を一つの進化史として再構成できたため重要だった。

**事実。** run 2 では、次の二つの順序づけられた event が支持された。

$$
e_1=\text{nonreciprocal parasitic exploitation before/by }90{,}000
$$

$$
e_2=\text{partner-contingent replication discrimination by }680{,}000
$$

これは有限の repeated AFN であり、二つの distinct functional event が同じ history に存在するという強い結果だった。一方、第三の distinct event は確認されなかった。

ここで arms race と functional-class expansion を同一視しなかったことが重要である。寄生者と防御側が配列、toggle、binding、copying strategy を更新し続けても、役割が exploitation と partner discrimination / defense の範囲内なら、それは既存 class 内の適応である。

$$
\text{arms-race elaboration}
\neq
\text{functional-class expansion}
$$

### 6.3 static-history analysis――literature work から一歩だけ出た場所

Stringmol の deposit には、すでに生成・処理された8 run の historical data があった。これを read-only で解析したのは、文献記述だけでは、後半に第三の event 候補が隠れているかを十分に攻撃できなかったためである。

**事実。** この作業は simulation ではない。Stringmol を実行・compile せず、parameter を変えず、新しい evolutionary history を生成せず、元の preprocessing pipeline も再実行しなかった。deposit 済みの species / reaction table を検査し、既存の frozen AFN criteria のもとで candidate event を再構成しただけである。

解析は reciprocal dependence が実在し、run 1 と run 6 では長く優勢になり得ることを確認した。しかし、それは早い時点ですでに出現した role の recurrence であったり、run 2 の (e_2) より前に成立したり、後発例では adaptive establishment が不足したりした。したがって結論は変わらなかった。

$$
\boxed{
\text{two-event AFN record remained the strongest claim}
}
$$

この negative result は、Stringmol に第三の event を生む能力がないという意味ではない。観察は右打ち切り・区間打ち切りされ、deposit の semantics が捉えない機能もあり得る。正確な主張は、再構成可能な deposit 内で (e_3) が支持されなかった、である。

### 6.4 positive-case search から event-history methodology へ

Stringmol、Avida、Geb を同じ logical criterion で比較すると、強い within-history count はそれぞれ 2、1、1 だった。Avida では EQU を含む logic-mediated resource acquisition の一つの function family が強く支持されたが、別実験の division of labor を同じ history に継ぎ足すことはできなかった。Geb では dominant social strategy の一 event は支持できたが、後の rebel は adaptation と class distinction が十分に解像されなかった。

**解釈。** この時点で、さらに positive case の名前を探すより、何を一つの event history として保持すべきかが中心問題になった。AFN program は system ranking から event-history methodology へ移った。

$$
\text{detection}
\rightarrow
\text{reconstruction}
\rightarrow
\text{validation}
$$

generic activity measure や persistence filter は候補を検出できる。次に、system-specific semantics、ancestry、interaction、carrier を用いて何が起きたかを再構成する。最後に N/F/H/A/C、provenance、deduplication、censoring、class relation によって claim を検証する。この三層を分けることで、検出された活動をそのまま adaptive novelty と呼ぶ誤りを避けた。

functional-class reasoning も次の三段階へ整理された。

$$
\text{activity}
\rightarrow
\text{causal role}
\rightarrow
\text{adaptive consequence}
$$

class identity の中心は causal role であり、adaptive consequence は独立の A evidence だった。機能を fitness outcome で定義すると、F と A が循環してしまう。比較は universal taxonomy ではなく、context、explanatory target、resolution を固定した pairwise な `SAME / DISTINCT / UNRESOLVED` relation とされた。

### 6.5 AFN を止めた本当の理由

AFN は、AFN が存在しないと分かったために止まったのではない。有限の AFN は Stringmol で支持された。また methodology が破綻したためでもない。event-history workflow は frozen corpus の Stringmol、Avida、Geb に system-specific な論理例外なしで適用でき、conditionally validated と判断された。

最終的な boundary は次だった。

$$
\boxed{\text{external independent validation}}
$$

functional-class の decisive edge を、scheme development から独立した domain-literate coder が、同一の blinded packet に対して adjudication 前に分類した記録は存在しなかった。内部で一貫して再適用できることと、independent reproducibility は違う。

同じ、または近縁の LLM を複数回呼ぶことも scientific independence ではない。共有された training history、model priors、protocol wording、context がある以上、別 sample は独立した科学者ではない。AI agent は adversarial critique、protocol debugging、literature retrieval、sensitivity analysis には使えるが、外部独立 validation を自己生成する装置ではない。

したがって AFN は、**METHOD PHASE COMPLETE, EXTERNAL VALIDATION PENDING** として pause した。これは理論的失敗ではなく、必要な人間的・外部的 validation resource が repository 内に存在しないという境界だった。

## 7. Complexity program――増えたものと、増え続けられるものを分ける

### 7.1 AFN の次に complexity を選んだ理由

AFN の停止後、complexity growth が選ばれた。これは AFN の代用品ではなく、OEE literature が独立に重視してきたもう一つの behavioral hallmark だった。また Geb には active-gene complexity と resource scaling に関する定量的 anchor があり、Hintze と Evoloops には false positive を攻撃する control があった。transformational novelty よりも、既存 published evidence のもとで object、trend、ceiling、scaling を区別しやすかった。

最初の firewall は単純だった。

$$
\boxed{\text{size}\neq\text{complexity}}
$$

genome length、parameter count、圧縮困難性、未使用 code、外部から増やした resource ceiling は、それだけでは意味のある complexity ではない。対象は system ごとに宣言された、causally active な entity organization または realized interaction organization でなければならなかった。

次の分離が program の中心になった。

$$
\boxed{
\text{realized complexity growth}
\neq
\text{resource scalability}
}
$$

時間 history の中で実際に complexity frontier が伸びたことと、資源上限を系統的に増やした family の中で、進化がより高い frontier に到達できることは異なる evidence object である。前者を (S)（sustainedness）、後者を (I)（indefinite/resource scalability）として別記録にした。

### 7.2 Avida、Aevol、Geb の異なる evidence role

これらを「どの system が最も OEE か」という ranking として読むと、program の意味を失う。それぞれは異なる証拠上の役割を担った。

**Avida。** fixed finite task environment の中で、genomic environmental information と complex-feature lineage を通じ、realized within-history complexity growth を示した。これは、進化史の中で complexity が実際に獲得されたという anchor である。一方、有限 task family と capacity limit があり、resource scalability は示さなかった。

**Aevol。** active functional proteome を対象に、replicated long lineage で complexity の蓄積と保持、すなわち ratchet の強い例を与えた。frozen result は

$$
\boxed{(S2,I0)}
$$

だった。extended realized growth は強いが、apparent bound があり、同じ complexity object の resource-scaling evidence はなかった。

**Geb。** active developmental gene count を用い、world/population と neural limit の両方を co-scale したときに、到達 complexity frontier が tested range で上昇することを示した。これは resource-scalable complexity frontier の anchor であり、frozen result は

$$
\boxed{(S1,I4)}
$$

だった。ただし I4 は **qualified published operational sense, to the extent tested** である。数学的な (K_\Pi(R)\to\infty) の証明でも、一つの fixed world で (C(t)\to\infty) を観察した結果でもない。

### 7.3 中心的な empirical structure――空いた conjunction

最も重要だったのは、強い (S) と強い (I) を同じ defensible complexity object、compatible protocol、同じ system で確認できなかったことである。

$$
\boxed{\text{strong }S+\text{strong }I}
$$

Aevol と Avida は realized growth 側を強くし、Geb は scalability 側を強くした。しかし一方を他方へ読み替えることはできなかった。長い history は scalability ではなく、resource-scaled family は fixed-regime ongoingness ではない。

正確な frozen statement は次だった。

> **NO STRONG CONJUNCTION CASE FOUND IN THE REVIEWED SEARCH SPACE.**

これは「そのような system は存在しない」という universal absence claim ではない。search は有限で publication-censored であり、空いた cell は reviewed evidence map の性質である。それを一つの missing mechanism の証拠とも解釈しなかった。

### 7.4 Complexity を止めた理由

Complexity methodology ((S,I)) は、Avida、Geb、Tierra、Hintze、Stringmol など異なる system と adversarial control に適用され、system-specific logical exception なしで retrospective validation された。したがって停止理由は measurement methodology failure ではない。

停止理由は、method が要求する強い conjunction exemplar が reviewed evidence に存在しなかったことである。Geb の time-resolved same-object fixed-resource history、または Aevol の same-object resource-scaling series のような、classification を変え得る empirical record は published corpus に含まれていなかった。

$$
\boxed{
\text{method retrospectively validated}
+
\text{strong conjunction exemplar absent}
}
$$

このため Complexity program は **EVIDENCE PHASE COMPLETE, EXEMPLAR MISSING** として pause した。

## 8. Exemplar program――部分的成功と broad OEE を分ける

### 8.1 exemplar scarcity は repository の新理論ではない

AFN と Complexity を終えると、中心問題は mechanism より一段上の evidence structure に移った。複数の system は明確な部分問題を解いているのに、それらを広い OEE claim として結び付けられる一つの model–measure–interpreted-result package が見つからなかった。

Bedau 2024 は Kuhnian exemplar を、研究を組織し、method と tacit standard を伝え、研究者を訓練する concrete problem–solution として論じていた。2024 OEE editorial も OEE exemplar の relative dearth を field problem として明示していた。

**事実。** したがって exemplar scarcity 自体は既知であり、repository が発見した新理論ではない。repository が行ったのは、この既知の問題を AFN と Complexity の evidence chain に即して具体化し、phenomenon、evidence/recording、validation、consensus、conjunction の異なる gap に分解したことだった。

### 8.2 component exemplars は「失敗した OEE systems」ではない

component scientific exemplar は、OEE 全体の成功例ではなくても、特定の科学問題に対する明確で再利用可能な model–method–result package である。

- **Evoloops:** constructive な自己複製 CA organism における Darwinian evolution。
- **Stringmol:** continuous history から再構成された finite repeated AFN。
- **Avida:** bounded environment 内の realized complexity evolution と complex-feature origin。
- **Aevol:** active functional complexity の accumulation / ratchet。
- **Geb:** active-individual complexity の resource scalability。
- **Flow-Lenia:** mass-conservative continuous substrate における rich morphological evolutionary dynamics と endogenous parameters。
- **Outlier:** causal ancestry を伴う emergent hierarchical self-replication。
- **Genelife:** selected configuration における sustained detected evolutionary activity と豊かな spatial/genetic dynamics。

これらは「OEE に失敗した system」ではない。replication、evolution、finite AFN、realized complexity、scalability、continuous dynamics、multiscale ancestry といった部分問題を切り出し、何をどこまで示せるかを教える scientific exemplar である。価値を OEE の完全達成だけで測ると、各 system の実際の科学的貢献を消してしまう。

### 8.3 broad exemplar が無い、という限定された結論

EX1 の結論は次だった。

> **COMPONENT EXEMPLAR SET ESTABLISHED, BROAD EXEMPLAR ABSENT.**

$$
\boxed{\text{OEE の部品については成功例がある}}
$$

一方で、reviewed fixed set では、ongoing AFN、strong complexity conjunction、あるいは他の一つの defensible OEE category を十分強く満たす broad artificial-OEE exemplar は確立しなかった。

$$
\boxed{
\text{それらを強く結合した人工進化の例は}
\atop
\text{現在の reviewed evidence では確立していない}
}
$$

これは broad exemplar の不存在証明ではない。また、すべての OEE category を同じ深さで調べたという意味でもない。leading evidence が Stringmol、Aevol、Geb に直交的に分かれていたため、どれか一つを global winner と呼ばなかった。

### 8.4 EX2――再現可能性、監査可能性、exemplar status

Exemplar program の次の問いは、将来ある candidate が現れたとき、後から claim を作り替えずに何を保存すれば、その OEE-relevant claim を監査できるかだった。

ここで三つを分けた。

$$
\boxed{
\text{reproducibility}
\neq
\text{claim auditability}
\neq
\text{exemplar status}
}
$$

model と experiment を再実行できても、measure が主張する対象を意味するとは限らない。evidence chain を監査できても、独立研究者が同じ interpretation に合意するとは限らない。さらに reproducible かつ auditable でも、community に共有される exemplar になったとは限らない。

MIASE、SED-ML、FAIR は model identity、procedure、parameter、provenance、accessibility、machine-readable record といった一般的 practice をすでに提供していた。EX2 はそれらを再発明しなかった。追加したのは、history identity、measure semantics、raw→processed→measure→claim trace、endogenous/exogenous intervention、censoring、trivial alternatives、run selection、interpretive validation といった OEE-specific な結び付けだった。

$$
\boxed{
\text{OEE-specific claim-to-evidence trace}
}
$$

形は、compact common core、claim-specific module、separate validation record の組み合わせだった。これは OEE definition でも community standard でもなく、repository guidance としての evidence integration だった。

### 8.5 EX2A――古い研究へ未来の checklist を押し付けない

EX2A では、この prospective specification を過去の8 systems・9 packages に逆適用した。目的は compliance test ではなく、specification 自体が本当に有用かを検証することだった。

$$
\boxed{\text{2026年の checklist を古い論文へ押し付けない}}
$$

古い CA 研究に Git、Docker、JSON、hash、dataset DOI がないことは、それだけで科学的欠陥ではない。paper、rule table、initial condition、figure、later archive に情報が分散していても、claim-relevant relation が意味的に再構成できればよい。`PARTIALLY AUDITABLE` は original publication が invalid という意味ではない。

**事実。** retrospective audit の結果は、**LOW BUREAUCRATIC OVERHEAD**、**ZERO LOGICAL SUBSTRATE EXCEPTIONS**、そして **RETROSPECTIVELY VALIDATED AS REPOSITORY GUIDANCE** だった。discrete CA、artificial chemistry、digital organism、evolving neural agent、continuous CA の違いによって common core を論理的に変更する必要はなかった。

同時に、この specification が phenomenon を作れないことも明確になった。記録を良くしても ongoing AFN や strong (S/I) conjunction は発生しない。独立 validator や community uptake も checklist からは生まれない。evidence infrastructure の完成は、exemplar gap の解決ではなかった。

## 9. 最終的な境界――一つではない empirical blockage

SYNTHESIS 008 の中心判断は次だった。

$$
\boxed{
\textbf{G8-A — GLOBAL LITERATURE/METHODOLOGY PHASE COMPLETE,}
\atop
\textbf{EMPIRICAL BOUNDARY REACHED}
}
$$

これは「データが足りない」という一語で潰せる状態ではない。境界は次のように異質だった。

$$
\boxed{\text{HETEROGENEOUS EMPIRICAL BOUNDARIES}}
$$

### 9.1 AFN の境界

AFN には finite positive phenomenon と、conditionally validated な event-history method がある。直近の不足は、同一 frozen packet を用いた **外部独立 validation resource** である。より強い ongoingness claim には、さらに豊かな長期 event history も不足している。

### 9.2 Complexity の境界

Complexity には realized growth と resource scalability の別々の positive evidence があり、((S,I)) method も retrospectively validated である。不足は、同じ object と compatible protocol に対する **strong-(S) / strong-(I) conjunction exemplar** である。

### 9.3 Broad OEE の境界

Broad OEE には component exemplar の mosaic がある。不足は、長い continuous history の中で複数の強い OEE-relevant dimension、または一つの compelling な declared OEE category を監査可能に示す **broad artificial exemplar** であり、さらに mechanism 推論に必要な matched positive/negative contrast である。

この三つは、それぞれ validator、same-object empirical record、multi-dimensional phenomenon / contrast の不足である。同じ failure mode ではなく、したがって一つの missing mechanism を暗示しない。

## 10. なぜ mechanism research に進まなかったか

mechanism inference に必要な gate は、おおむね次の conjunction とされた。

$$
\boxed{
\text{stable phenomenon}
+
\text{credible positive exemplar}
+
\text{meaningful negative/matched contrast}
+
\text{causal discriminability}
}
$$

**事実。** repository はこの conjunction を満たさなかった。とくに不足していたのは、credible positive exemplar と matched contrast である。

Aevol ((S2,I0)) と Geb ((S1,I4)) の対照は informative だが、substrate、complexity semantics、selection、resource structure、protocol がすべて違う。これは axis split を示す descriptive comparison であり、causal contrast ではない。同様に Evoloops、Stringmol、Aevol、Geb の component mosaic を合わせても、一つの mechanism は同定できない。

したがって最終判断は **NOT READY FOR MECHANISM** だった。これは mechanism が存在しないという結論ではなく、現在の evidence から mechanism を識別する準備ができていないという判断である。

## 11. なぜ implementation しなかったか

最終判断は **IMPLEMENTATION NOT JUSTIFIED** だった。

$$
\boxed{\text{Rust で実装できない、という意味ではない}}
$$

問題は能力ではなく研究上の正当化だった。simulation や system construction は可能でも、どの positive regime と negative regime を作り、何を intervention し、どの結果が競合説明を分けるのかが定まっていなかった。

$$
\boxed{
\text{何を実装すれば重要な科学的問いを識別できるか}
\atop
\text{まだ十分に決まっていない}
}
$$

この状態で architecture を選べば、最初に惹かれた Evoloops–Lenia–autopoiesis synthesis を、evidence acquisition の名で再開する危険があった。rich behavior が得られても、なぜ得られたか、何と比べるべきかが不明なままになる。実装能力と実装の科学的 justification を分離したことが、この研究の重要な停止判断だった。

## 12. なぜ transformational novelty を始めなかったか

H2 transformational novelty は未解決であり、historical descriptive-model escape という distinct residue を持っていた。それでも開始しなかった。

$$
\boxed{\text{未研究}\neq\text{今もっとも情報価値が高い}}
$$

**事実。** strong classification には、candidate event より前に scientifically justified な descriptive model / meta-model が frozen されているか、独立に強く制約できる必要がある。既存 candidate は retrospective interpretation が中心で、記述を粗くすれば escape を作れ、豊かにすれば escape を隠せる observer-contract problem が大きかった。また Q006、Q016、F1/F2、major transitions、compositionality と重なる危険も高かった。

有限の transformational event を一つ分類しても、ongoing transformational novelty や AFN/complexity の causal contrast deficit は直ちには変わらない。継続条件は topic coverage を埋めることではなく、research state を変えられることだった。H2 は科学的には重要でも、2026年9月時点では current state-changing value が低いと判断された。

## 13. `HYPOTHESES.md = \varnothing` という成果

最終状態は次だった。

$$
\boxed{\texttt{HYPOTHESES.md}=\varnothing}
$$

SYNTHESIS 008 の判定は **H2 — HYPOTHESIS GENERATION PREMATURE FOR EMPIRICAL REASONS** である。ここでの H2 は hypothesis-file audit の decision label であり、transformational novelty hallmark H2 とは別物である。

**解釈。** 仮説が思いつかなかったのではない。候補を empirical discrimination の手前で意図的に昇格させなかった。AFN には finite positives があったが、独立 validation と long/matched histories がない。Complexity には強い component evidence があったが、same-object conjunction がない。Exemplar matrix は mosaic を与えたが causal comparability を与えなかった。

$$
\boxed{
\text{仮説候補を empirical discrimination の手前で}
\atop
\text{意図的に昇格させなかった}
}
$$

空の hypothesis file は、研究が何も生まなかった印ではない。novelty firewall、prior-art firewall、contrast gate が機能し、もっともらしい物語を結果として保存しなかったという negative accomplishment である。

## 14. Codex / agent research loop から学んだこと

この研究は OEE についてだけでなく、agent を使って長期研究を進める方法についても多くを教えた。

### LLM context は working memory、repository は persistent scientific memory

一回の context は、比較、批判、文章化には強いが、研究史全体を安定して保持する場所ではない。repository が、確立事項、未確定 reasoning、反例、停止理由、provenance を外部化する persistent scientific memory になった。重要なのは大量に保存することではなく、canonical state へ安定知識を圧縮し、不確実な reasoning には必要な粒度を残すことだった。

### 一回一問・一 operation

一度に system search、mechanism generation、formalization、implementation を行うと、どの evidence がどの判断を支えたのかが崩れる。一回一問、一つの operation に絞ることで、入力、判断、stop condition、次へ進めない理由を追跡できた。

### stop condition を毎回明示する

agent は、答えが弱いと次の細分化を自然に生成できる。それを防いだのが stop condition だった。criterion が安定し、残りが unrecorded history や external coder に依存すると判明したら、理論問題をさらに細くして延命しない。停止は失敗後の処理ではなく、research design の一部だった。

### closed branch を別名で再開しない

`generativity`、`organizational type`、`selection structure`、`self-maintaining plasticity` のような語は、別名で closed branch を再開する入口になり得た。terminology audit と containment map によって、用語が新しいだけで内容が既知という事態を抑えた。

### synthesis pass で repository entropy を圧縮する

各 Q-note は provenance を持つが、その数が増えると研究状態そのものが読めなくなる。SYNTHESIS 001–008 は、逐次履歴を dependency graph、terminal labels、boundary statement に圧縮した。これは単なる要約ではなく、過去の分岐を再び active frontier と誤認しないための entropy control だった。

### agent の速度が人間の理解を追い越さない

agent は文献、反例、分類、次の問いを人間より速く生成できる。その速度は利点である一方、人間が概念の変化を内面化する前に repository だけが先へ進む危険を生む。consolidation と pause は、agent の throughput を落とすためではなく、人間の理解と研究状態を再同期させるためにも必要だった。

### implementation と research justification を分離する

code を書けること、simulation を回せること、architecture を設計できることは、どの結果が科学的に識別的かとは別である。この区別がないと、実装の進捗が理論的進捗の代理になってしまう。

### AI agents を independent scientific validators と見なさない

複数回の agent call、別 prompt、別 sampling は、科学的独立性を自動的に作らない。AI の provenance、共有 prior、scheme exposure を明示し、independent validation は外部の人間的・制度的 resource として扱う必要があった。

## 15. Agent を使ったことで良くなったこと

**解釈。** agent workflow は、とくに「候補を作る」より「候補を壊す」局面で有効だった。

- 文献と prior art を高速に突き合わせ、魅力的な説明を既存概念へ戻せた。
- counterexample を繰り返し生成し、単純な含意を早い段階で破壊できた。
- 同じ内容が異なる terminology で再出現する terminology proliferation を検出できた。
- N/F/H/A/C、(S/I)、P/E/V/C/J のように claim を evidence link へ分解できた。
- repository-level state management により、closed branch、paused program、unblock condition を区別できた。
- 毎 pass で hypothesis firewall を再適用し、もっともらしいが識別不能な causal story の固定化を防げた。

とくに価値があったのは、棄却を「成果なし」と扱わず、どの inference がなぜ通らないかを provenance とともに保存できた点である。

## 16. Agent を使うことで生じ得た危険

同じ workflow は、制御しなければ研究を見かけ上だけ延命できる。

- **「次がある」ためだけの continuation:** どの結果からも次の問いを生成できるため、state-changing value がなくても研究が続いてしまう。
- **terminology proliferation:** 新語が novelty の感覚を作り、既知理論の再包装を発見に見せる。
- **phenomenon のない methodology:** positive phenomenon が薄いまま、checklist、taxonomy、robustness protocol だけが精緻化する。
- **false novelty:** prior-art search より先に仮説らしい名前を与えると、既知概念との差が見えなくなる。
- **repository entropy:** artifact が増えるほど、過去の local decision が current state に見える。
- **agent-produced confidence:** 整った文章、数式、表は evidence strength 以上の確信を演出できる。
- **human understanding lag:** agent の処理速度に人間の理解が追いつかず、なぜその判断になったかを repository から読み戻せなくなる。

これらを抑えるため、STOP、consolidation、canonical compression、one-operation rule を重視した。とくに、方法論をさらに精緻化しても phenomenon、validator、matched contrast を作れないと分かった時点で、継続そのものを疑う必要があった。

## 17. 「研究が進んだ」の定義が変わった

初期には、進歩は次のように見えやすかった。

$$
\boxed{\text{new mechanism / implementation}}
$$

何かを作り、新しい mechanism name を得れば、問題に近づいたと感じられた。しかし実際の研究では、より多くの前進が negative form を取った。

$$
\boxed{\text{誤った問いを閉じる}}
$$

$$
\boxed{\text{推論してはいけない境界を特定する}}
$$

$$
\boxed{\text{次に必要な evidence class を明示する}}
$$

**解釈。** 理論候補を prior art に吸収し、measurement problem と mechanism gap を分離し、finite observation から incapacity を推論しないことも research progress だった。空の hypothesis file、実装しなかったこと、最後に pause したことは、活動量を成果と同一視しないという研究観の変化を表している。

## 18. 現時点で言える最も大きなこと

過剰主張を避けてまとめるなら、最大の到達点は次である。

$$
\boxed{
\text{OEE の一般 mechanism はまだ分からない。}
\atop
\text{しかし、現在の artificial-evolution evidence から}
\atop
\text{mechanism を推論するために欠けているものは、}
\atop
\text{かなり具体的に分離された。}
}
$$

欠けているものは一語の「データ」ではない。AFN では external independent validation と richer event history、Complexity では same-object strong (S/I) evidence、Broad OEE では compelling auditable exemplar と matched causal contrast である。

また、artificial evolution に成果がないわけでもない。Darwinian self-reproduction、finite repeated AFN、realized complexity accumulation、resource scalability、continuous morphological dynamics、hierarchical self-replication には、それぞれ強い component exemplar がある。分からないのは、それらがなぜ一つの系で持続的に結び付くのか、あるいは結び付く必要があるのかである。

## 19. 現時点で言えないこと

この repository の evidence から、次のことは言えない。

- OEE の一般的・必要十分な mechanism。
- 自然進化が open-ended に見える一般的な原因。
- 人工進化が閉じる一般的な原因。
- ecology または niche construction が OEE の必要条件・十分条件であること。
- major transitions が OEE を生むこと、または transition が次の transition を一般に促進すること。
- complexity scalability が ongoing complexity growth や OEE を生むこと。
- autopoiesis、organizational closure、self-maintenance が OEE を生むこと。
- self-reference、universal construction、compositionality、meta-evolution が OEE を保証すること。
- Stringmol に第三の AFN event を生む能力がないこと。
- strong-(S) / strong-(I) artificial system が存在しないこと。
- broad artificial-OEE exemplar が世界に存在しないこと。
- Lenia / Flow-Lenia をどう改造すれば OEE が生じるか。
- Evoloops、Lenia、Autopoiesis をどう統合すればよいかという新しい system architecture。
- natural evolution と artificial evolution の差を因果的に説明する matched comparison。

これらの `NOT ESTABLISHED` は `DOES NOT OCCUR` ではない。

## 20. もし将来再開されたとしたら――当時知られていた unblock conditions

これは action plan ではない。2026年9月時点で、どの外部変化が現在の停止理由を変え得ると理解されていたかを記録する。

- AFN では、frozen blinded packet を scheme-independent かつ domain-literate な外部 coder が adjudication 前に独立分類した genuinely independent validation が得られた場合、現在の validation boundary は変化し得ると考えられていた。
- Complexity では、同じ defensible object に対して strong (S) の temporal evidence と strong (I) の resource-scaling evidence を compatible protocol で持つ package、または frozen method を適用できる新しい Geb / Aevol histories が得られた場合、empty conjunction の状態は変化し得ると考えられていた。
- Broad OEE では、明示された OEE category または複数 hallmark を、continuous history、censoring、nontriviality control、provenance とともに示す compelling artificial exemplar が現れた場合、exemplar boundary は変化し得ると考えられていた。
- Mechanism inference では、同一または closely matched system に OEE-positive と OEE-negative の regime があり、hallmark、history、opportunity、observation budget を揃えた causal/interventional contrast が得られた場合、`NOT READY FOR MECHANISM` の理由が変化し得ると考えられていた。
- Transformational novelty では、scientifically justified な descriptive model / meta-model が事前に frozen されるか、独立に十分制約され、model escape が非自明になる published evidence が現れた場合、当時の low state-changing value の判断が変化し得ると考えられていた。

これらは次に行うべき TODO ではなく、pause 時点で既知だった条件付きの歴史記述である。

## 21. 主要 artifact map

過去の詳細を人間が確認するときのために、研究の転換点を担った artifact だけを挙げる。これは current state の入口ではない。

1. [`SYNTHESIS_001_Q001_Q012.md`](../../SYNTHESIS_001_Q001_Q012.md) — replication、closure、capacity、accessibility、major transition の初期理論境界。
2. [`SYNTHESIS_002_Q013_Q021.md`](../../SYNTHESIS_002_Q013_Q021.md) — organizational type の domain-specific decomposition と Fernandes instrumentation boundary。
3. [`SYNTHESIS_003_Q022_Q027.md`](../../SYNTHESIS_003_Q022_Q027.md) — current theoretical decomposition boundary と hallmark-first への転換。
4. [`SYNTHESIS_004_AFN_HALLMARK_PROGRAM.md`](../../SYNTHESIS_004_AFN_HALLMARK_PROGRAM.md) — AFN evidence / methodology program の統合と external-validation boundary。
5. [`ANALYSIS_001_STRINGMOL_STATIC_HISTORY_REANALYSIS.md`](../../ANALYSIS_001_STRINGMOL_STATIC_HISTORY_REANALYSIS.md) — deposit 済み history の read-only analysis と two-event result の維持。
6. [`METHODOLOGY_001_AFN_EVENT_HISTORY.md`](../../METHODOLOGY_001_AFN_EVENT_HISTORY.md) — detection→reconstruction→validation を結ぶ AFN event-history workflow。
7. [`FORMALIZATION_001_AFN_FUNCTIONAL_CLASS_IDENTITY.md`](../../FORMALIZATION_001_AFN_FUNCTIONAL_CLASS_IDENTITY.md) — pairwise causal-role による functional-class comparison。
8. [`METHODOLOGY_002_AFN_INDEPENDENT_CODING_ROBUSTNESS.md`](../../METHODOLOGY_002_AFN_INDEPENDENT_CODING_ROBUSTNESS.md) — genuine independent coding の条件と停止境界。
9. [`SYNTHESIS_005_NEXT_OEE_HALLMARK.md`](../../SYNTHESIS_005_NEXT_OEE_HALLMARK.md) と [`SYNTHESIS_006_COMPLEXITY_HALLMARK_PROGRAM.md`](../../SYNTHESIS_006_COMPLEXITY_HALLMARK_PROGRAM.md) — complexity hallmark の選択と、Aevol/Geb split・conjunction gap の統合。
10. [`METHODOLOGY_003_COMPLEXITY_SUSTAINEDNESS_SCALABILITY.md`](../../METHODOLOGY_003_COMPLEXITY_SUSTAINEDNESS_SCALABILITY.md) — temporal sustainedness (S) と resource scalability (I) の分離。
11. [`EVIDENCE_MAP_003_COMPLEXITY_STRONG_S_STRONG_I_SEARCH.md`](../../EVIDENCE_MAP_003_COMPLEXITY_STRONG_S_STRONG_I_SEARCH.md) — expanded positive-case map と bounded search result。
12. [`SYNTHESIS_007_GLOBAL_OEE_EXEMPLAR_GAP.md`](../../SYNTHESIS_007_GLOBAL_OEE_EXEMPLAR_GAP.md) — component exemplar と broad exemplar の分離、既知の field-level exemplar gap。
13. [`EVIDENCE_MATRIX_004_OEE_CANDIDATE_EXEMPLARS.md`](../../EVIDENCE_MATRIX_004_OEE_CANDIDATE_EXEMPLARS.md) — fixed candidate set の model–measure–interpreted-result 比較。
14. [`SPECIFICATION_001_PROSPECTIVE_OEE_EXEMPLAR_EVIDENCE.md`](../../SPECIFICATION_001_PROSPECTIVE_OEE_EXEMPLAR_EVIDENCE.md) と [`VALIDATION_003_PROSPECTIVE_OEE_SPEC_RETROSPECTIVE_AUDIT.md`](../../VALIDATION_003_PROSPECTIVE_OEE_SPEC_RETROSPECTIVE_AUDIT.md) — OEE-specific prospective evidence integration と historical-fairness audit。
15. [`SYNTHESIS_008_GLOBAL_OEE_RESEARCH_BOUNDARY.md`](../../SYNTHESIS_008_GLOBAL_OEE_RESEARCH_BOUNDARY.md) — global literature/methodology completion、heterogeneous empirical boundaries、最終 pause。

## 22. この研究をここで止めた理由

最後に残った原則は、もっとも単純なものだった。

$$
\boxed{
\text{何かを続けること}
\neq
\text{研究を進めること}
}
$$

文献をもう一巡すること、methodology をもう一段精緻化すること、未研究 hallmark を一つ埋めること、simulation architecture を考えることは、いずれも活動にはなる。しかし、external validator、strong conjunction exemplar、broad positive history、matched causal contrast がない状態では、それらが central research state を変える見込みは低かった。

**事実。** 最終状態は次の通りだった。

- **literature/methodology phase complete**
- **empirical boundary reached**
- **mechanism not ready**
- **implementation not justified**
- **repository paused**

**解釈。** ここで止めたのは、OEE が解けたからでも、OEE が存在しないと分かったからでも、研究に価値がなかったからでもない。現在の材料で正当化できる推論を使い切り、それ以上を続けると、欠けている empirical object を言葉、method、architecture で代用し始める可能性が高くなったからである。

この pause は消極的な終点ではない。「何が分からないか」に加え、「何が得られるまでは、その分からなさを mechanism として語ってはいけないか」を確定した地点である。初期に期待した統合 system は作られなかったが、その代わりに、なぜ今それを作ることが科学的に早いのかが説明できるようになった。それが、この literature-only program が到達した最も誠実な完了形だった。

---

> **Canonical-state warning**
>
> この文書は retrospective archive であり、研究再開時の canonical state ではない。
>
> 研究再開時には必ず `STATUS.md`、`FRONTIER.md`、`KNOWN.md`、`AGENTS.md` を優先すること。

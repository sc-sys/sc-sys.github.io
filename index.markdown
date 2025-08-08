---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults
layout: my_default
---
  <link rel="stylesheet" href="{{ '/assets/css/default.css' | relative_url }}">
  <main class="page-content" aria-label="Content">

    <H3>趣旨</H3>
    <p>
      FPGAの普及、オープンソースの充実によりRISC-Vに代表されるような計算機システムが容易に作れるようになりました。計算機理論分野では現実社会に応用する研究が活発化しAWSなどでは実システムに供しています。一方で新しい原理を理論研究と共に計算機ハードウェアからソフトウェアのレイヤまで研究・開発するために必要な知識の獲得と議論の場が乏しいと我々は考えています。そこで、若手研究者・技術者の方々が学び議論できる場を設けることにしました。
    </p>
    <br>

    <H3><p style="line-height:0.3">主催</p></H3>
    <p>
      <A href="https://ds.rois.ac.jp/center9/">情報・システム研究機構 データサイエンス共同利用基盤施設 セキュアコンピュータシステム研究開発センター</A>
    </p>

    <h3><p style="line-height:0.3">世話人</p></h3>
    <ul style="line-height:1.1">
      <li>関山 太朗（国立情報学研究所／情報・システム研究機構）</li>
      <li>大畑 幸矢 (情報・システム研究機構)</li>
      <li>畑 輝史（慶應義塾大学）</li>
    </ul>

    <H3><p style="line-height:0.3">Keywords</p></H3>
    <UL style="line-height:1.1">
      <LI>TEE, Confidential Computing, Hypervisor, VM</LI>
      <LI>Formal Verification, Theorem Prover, SAT/SMT Solver</LI>
      <LI>RISC-V, Linux, Rust, ProVerif, Tamarin</LI>
    </UL>

    <H3><p style="line-height:0.3">対象</p></H3>
    <UL style="line-height:1.1">
      <LI> 学生、若手研究者・技術者、教育関係者</LI>
    </UL>

    <H3><p style="line-height:0.3">形式</p></H3>
    <UL style="line-height:1.1">
      <LI>当初は勉強会的に参加者の中から有志が発表し全員で議論。皆さんとの議論を大事にしたいので原則現地参加をお願いします。</LI>
      <LI>科研費における若手の定義は学位取得後8年未満の研究者としていますが、この定義にとらわれず、ここでは「若手」とは年齢問わず自らの自由な発想の元、研究・開発している・していきたい方々とします。</LI>
      <LI> 企画・運営していく若手ボランティアも募集しています。第1回ワークショップ参加登録フォームにご記入ください。</LI>
    </UL>

    <H3><p style="line-height:0.3">Slack</p></H3>
    <DIV>
      本ワークショップに関するご連絡，講演資料の共有，リモート参加・質疑には Slack を利用します．
      <A href="https://join.slack.com/t/satss/shared_invite/zt-39t7ge2af-gusWS~jXcL3FlHOkSNNG7A">こちら</A>の招待リンクからご参加ください．
    </DIV>

    <br>
    <H3><p style="line-height:0.3">今後の開催予定</p></H3>
    <UL class="workshop-list" style="line-height:1.1">
     <LI>
       <DT>第9回：セキュアシステムソフトウェア</DT>
       <DT>日時：2025年8月21日15:00〜17:00（開場14:30）</DT>
       <DT>開催場所：<A href="https://www.hit-u.ac.jp/hall/accessjp.html">一橋講堂 特別会議室101-103</A></DT>
       <DT>リモート参加：<A href="https://join.slack.com/t/satss/shared_invite/zt-39t7ge2af-gusWS~jXcL3FlHOkSNNG7A">Slack</A>にて連絡</DT>
       <OL>
         <LI>
           <DT>講演者：Gustavo A. R. Silva (The Linux Foundation)</DT>
           <DT>
           <DETAILS>
             <SUMMARY>講演者情報</SUMMARY>
             <DIV class="speaker-bio">
               Gustavo A. R. Silva works full-time as an Upstream Linux Kernel Engineer focused
               on hardening and proactive security. He has spent the past several years fixing
               all sorts of bugs and hardening the Linux kernel. His work is supported by The
               Linux Foundation and the Alpha-Omega project. He’s a member of the Linux Kernel
               Self-Protection Project and a regular speaker at Kernel Recipes and Open Source
               Summit. He has also presented at Linux Security Summit, Lund LinuxCon, Linux
               Plumbers Conference, Everything Open, The University of Adelaide, and Symposium
               sur la Sécurité des Technologies de l'Information et des Communications (SSTIC)
               as an invited speaker.
             </DIV>
           </DETAILS>
           </DT>
           <DT>講演タイトル：Enhancing spatial safety: Better array-bounds checking in C (and Linux)</DT>
           <DT>
           <DETAILS>
             <SUMMARY>概要</SUMMARY>
             <DIV class="abstract">
               The C language has historically suffered from a lack of proper bounds-checking
               on all kinds of arrays. The Linux Kernel Self-Protection Project has been
               addressing this issue for several years. In this presentation, we will learn
               about the most recent hardening efforts to resolve the problem of bounds-checking,
               particularly for fixed-size and flexible arrays.
               We will explore the different mechanisms being used to harden key APIs like
               memcpy() against buffer overflows, which includes the use of some interesting
               built-in compiler functions. We will also talk about a couple of recent compiler
               options like -fstrict-flex-arrays and -Wflex-array-member-not-at-end, as well
               as the new counted_by attribute released in Clang 18 and GCC 15, which helps us
               gain run-time bounds-checking coverage on flexible arrays.
               Overall, we will discuss how various challenges have been overcome, and highlight
               the innovations developed to solve the problem of array bounds-checking in both C
               and the Linux kernel once and for all.
             </DIV>
           </DETAILS>
           </DT>
         </LI>
         <LI>
           <DT>講演者：Keita Suzuki (Keio University)</DT>
           <DT>タイトル：Balancing Analysis Time and Bug Detection: Daily Development-friendly Bug Detection in Linux</DT>
           <DT>
           <DETAILS>
             <SUMMARY>概要</SUMMARY>
             <DIV class="abstract">
               Linux, a battle-tested codebase, is known to suffer from many bugs despite its extensive testing mechanisms. While many of these bugs require domain-specific knowledge for detection, a significant portion matches well-known bug patterns. Even though these bugs can be found with existing tools, our simple check of Linux kernel patches suggests that these tools are not used much in the developer's daily workflow. The lack of usage is probably due to the well-known trade-off between analysis time and bug detection capabilities: tools typically employ complex analysis to effectively and comprehensively find bugs in return for a long analysis time, or focus on a short analysis time by only employing elementary analyses and thus can only find a very limited number of bugs. Ideally, developers expect the tools to incur short analysis time, while still finding many bugs to use them in daily development.
               This paper explores an approach that balances this trade-off by focusing on bugs that can be found with less computationally-complex analysis methods, and limiting the scope to each source code. To achieve this, we propose a combination of computationally lightweight analyses and demonstrate our claim by designing FiTx, a framework for generating daily development-friendly bug checkers that focus on well-known patterns. Despite its simplicity, FiTx successfully identified 47 new bugs in the Linux kernel version 5.15 within 2.5 hours, outperforming Clang Static Analyzer and CppCheck in both speed and bug detection. It demonstrates that focusing on less complex bug patterns can still significantly contribute to the improvement of codebase health. FiTx can be embedded into the daily development routine, enabling early bug detection without sacrificing developers' time.
             </DIV>
           </DETAILS>
           </DT>
         </LI>
       </OL>
     </LI>

     <li>
       <dt>第10回：システムソフトウェアと形式検証</dt>
       <dt>日時：2025年9月1日</dt>
       <dt>開催場所：東京 品川（会場は決まり次第お知らせします）</dt>
       <br />
       <dt>予定講演（講演者氏名順）</dt>
       <ol>
         <li>
           <dt>石川 裕（大妻女子大学／情報・システム研究機構）</dt>
           <dt>TriniTEE プロジェクト：ハードウェア・ソフトウェア・理論の連携によるユニバーサル TEE アーキテクチャの実現</dt>
         </li>
         <li>
           <dt>海野 広志（東北大学）</dt>
           <dt>Toward Automated Verification of Low-Level Programs in C and Rust via Fixpoint Logic Solvers</dt>
         </li>
         <li>
           <dt>織田 幸弘（東北大学）</dt>
           <dt>セキュリティ束の動的拡張が可能なπ計算の型ベース情報流解析</dt>
         </li>
         <li>
           <dt>内藏 理史（早稲田大学）</dt>
           <dt>Ranking and Invariants for Lower-Bound Inference in Quantitative Verification of Probabilistic Programs</dt>
         </li>
         <li>
           <dt>佐藤 重幸（電気通信大学）</dt>
           <dt>検証付きコンパイラ最適化の発展</dt>
         </li>
         <li>
           <dt>佐藤 哲也（東京科学大学）</dt>
           <dt>差分プライバシーの形式化とf-divergenceの形式化について</dt>
         </li>
         <li>
           <dt>関山 太朗（国立情報学研究所／情報・システム研究機構）</dt>
           <dt>階層化された計算機システムのセキュリティ検証と課題</dt>
         </li>
         <li>
           <dt>冨田 尭（北陸先端科学技術大学院大学）</dt>
           <dt>自動運転システムの体系的形式検証に向けて</dt>
         </li>
         <li>
           <dt>服部 穣（東京大学）</dt>
           <dt>Automated Detection of Reference Counting Bugs in Linux Kernel Drivers</dt>
         </li>
         <li>
           <dt>西村 啓佑（Inria-Paris ソルボンヌ大学）</dt>
           <dt>Linuxカーネルのスケジューラに対する形式検証の取り組み</dt>
         </li>
         <li>
           <dt>蓮尾 一郎（国立情報学研究所）</dt>
           <dt>形式手法の実世界応用を目指して： モデル不在問題への理論的アプローチ</dt>
         </li>
         <li>
           <dt>Cheng-Hui Weng（名古屋大学）</dt>
           <dt>An Approach to Formalize Information-theoretic Security of Multiparty Computation Protocols Across Cryptographic Paradigms</dt>
         </li>
       </ol>
     </li>

     <li>
       <dt>第11回：理論関連のトピック（具体的な内容は調整中）</dt>
       <dt>話者：大堀 淳（情報・システム研究機構），佐藤 重幸（電気通信大学）</dt>
       <dt>日時：2025年10月ごろ</dt>
       <dt>開催場所：未定</dt>
     </li>
     <li>
       <dt>第12回：ハードウェア関連のトピック（具体的な内容は調整中）</dt>
       <dt>話者：内山 一秀（情報・システム研究機構），他調整中</dt>
       <dt>日時：2025年12月ごろ</dt>
       <dt>開催場所：未定</dt>
     </li>
     <li>
       <dt>第13回：未定</dt>
       <dt>話者：未定</dt>
       <dt>日時：2026年3月ごろ</dt>
       <dt>開催場所：未定</dt>
     </li>
    </ul>

    <hr style="height:3px">
    <H4><p style="padding-bottom:0px">終了したワークショップ</p></H4>
    <UL class="workshop-list" style="line-height:1.1">
     <LI margin-top="1px" margin-bottom="1px">
       <DT>第8回："Cloud Server Security: From Trusted Execution Environment (TEE) to Fully Homomorphic Encryption (FHE)"</DT>
       <DT>話者：<A href="https://sites.google.com/view/arpers" target="_new">Yan Solihin</A></DT>
       <DT>日時：2025年6月3日(火)16:30〜18:30</DT>
       <DT>開催場所：<A href="https://www.waseda.jp/inst/gcs/access/" target="_new">早稲田大学グリーン・コンピューティング・システム研究開発センター (40号館) 1階プレゼンテーションルーム</A></DT>
       <!-- <DT>リモート参加可能（開催前日にメールでURLを送付）</DT> -->
       <DT>
         <DETAILS>
           <SUMMARY>概要</SUMMARY>
           <DIV>
             In this talk I will discuss the ongoing challenges for ensuring the confidentiality and integrity of computation in the cloud servers.
             In the first part of the talk, I will discuss the drawbacks of current Trusted Execution Environment (TEE) designs.  TEE protects sensitive applications in the cloud with the minimal trust in the cloud provider. Existing TEEs with integrity protection however lack support for data management primitives, causing data sharing between enclaves either insecure or cumbersome. This paper proposes a new data abstraction for TEEs, data enclave. As a data-centric abstraction, data enclave is decoupled from an enclave’s existence, is equipped with flexible secure permission controls, and crytographically isolated. It eliminates the hurdles for enclaves to cooperate efficiently, and at the same time, enables dynamic shrinking of the height of integrity tree for performance. This paper presents this new abstraction, its properties, and the architecture support. Experiments on synthetic benchmarks and three real-world applications all show that data enclave can help improve the efficiency of enclaves and inter-enclave cooperations significantly while enhancing the security protection.
             In the second part of the talk, I will discuss our research in Fully Homomorphic Encryption (FHE) verifiability. FHE allows computations to be performed directly on encrypted data without needing to decrypt it first. This “encryption-in-use” feature is crucial for securely outsourcing computations in privacy-sensitive areas such as healthcare and finance. Nevertheless, in the context of FHE-based cloud computing, clients often worry about the integrity and accuracy of the outcomes. This concern arises from the potential for a malicious server or server-side vulnerabilities that could result in tampering with the data, computations, and results.  Ensuring integrity and verifiability with low overhead remains an open problem, as prior attempts have not yet achieved this goal. To tackle this challenge and ensure the verification of FHE’s private computations on encrypted data, we introduce DataSeal, which combines the low overhead of the algorithm-based fault tolerance (ABFT) technique with the confidentiality of FHE, offering high efficiency and verification capability.  Through thorough testing in diverse contexts,  we demonstrate that DataSeal achieves much lower overheads for providing computation verifiability for FHE than other techniques that include MAC, ZKP, and TEE. DataSeal’s space and computation overheads decrease to nearly negligible as the problem size increases.
           </DIV>
         </DETAILS>
       </DT>
     </LI>
     <LI> <DT>第7回：TEE関連研究動向</DT>
      	   <DT>日時：2024年7月1日(月)14:00〜17:00</DT>
 	   <DT>共催：早稲田大学グリーン・コンピューティング・システム研究機構</DT>
	   <DT>開催場所：<A href="https://www.waseda.jp/inst/gcs/access/" target="_new">早稲田大学グリーン・コンピューティング・システム研究開発センター (40号館) 1階プレゼンテーションルーム</A></DT>
	   <DT>　　　　　リモート参加可能（開催前日にメールでURLを送付）</DT>
	   <DT>定員：60名</DT>
	   <DT>話題：</DT>
	   <DT>　"CTR: Checkpoint, Transfer, and Restore for Secure Enclaves"</DT>
	   <DT>　　　Yoshimichi Nakatsuka (ETH Zurich)</DT>
 	   <DT>　"TDOS: Trustworthy Heterogeneous Disaggregated Architectures"</DT>
	   <DT>　　　Atsushi Koshiba (Technical University of Munich)</DT>
 	   <DT>　"OP-TEEの利用事例：OP-TEEを用いたIoTのための安全な階層鍵管理機構"</DT>
	   <DT>　　　竹房 あつ子 (NII)</DT>
     </LI>
     <LI> <DT>第6回：Arm TrustZone</DT>
      	   <DT>日時：2024年5月10日(金)13:00〜18:00</DT>
	   <DT>　　　セコムIS研究所とデータセンター見学：13:00〜15:30</DT>
	   <DT>　　　　　(企業の方は見学出来ません)</DT>
   	   <DT>　　　Arm TrustZone講義：15:30〜18:00</DT>
 	   <DT>共催：セコム（株）</DT>
	   <DT>開催場所：<A href="https://www.secom.co.jp/isl/contact/" target="_new">セコムIS研究所</A></DT>
	   <DT>　　　　　リモート参加可能（開催前日にメールでURLを送付）</DT>
	   <DT>講師：宮澤慎一（セコム（株））</DT>
	   <DT>概要：</DT>
      	   <DT>　　1) ARMとTrustZoneの概要</DT>
       	   <DT>　　2) Global Platformの概要</DT>
	   <DT>　　3) OP-TEEの解説</DT>
	   <DT>　　4) OP-TEEプログラミングハンズオン</DT>
	   <DT>ハンズオンではQEMUを使います。ノートPCをご持参ください。あらかじめソフトウェアをインストールしておいてください。詳細は追って連絡します</DT>
	   <DT>定員：100名（見学は30名）</DT>
     </LI>
     <LI> <DT>第4回&第5回：形式検証入門、メモリ暗号化・整合性検証の最近動向</DT>
      	   <DT>日時：2024年3月8日(金)15:00〜18:00</DT>
 	   <DT>共催：早稲田大学グリーン・コンピューティング・システム研究機構</DT>
	   <DT>開催場所：<A href="https://www.waseda.jp/inst/gcs/access/" target="_new">早稲田大学グリーン・コンピューティング・システム研究開発センター (40号館) 1階プレゼンテーションルーム</A></DT>
	   <DT>　　　　　リモート参加可能（開催前日にメールでURLを送付）</DT>
	   <DT>講師：関山太朗（国立情報学研究所）</DT>
   	   <DT>　　　高前田伸也（東京大学）</DT>
	   <DT>定員：60名</DT>
    </LI>
    <LI>
 	<DL>
		<DT>第3回：Virtualization 最近動向 RISC-V Virtualization, Intel TDX, Arm CCA</DT>
		<DT>日時：2024年2月1日(木)16:00〜18:00</DT>
		<DT>開催場所：国立情報学研究所 1208-1210会議室</DT>
		<DT>　　<A HREF="https://www.nii.ac.jp/about/access/">東京都千代田区一ツ橋2-1-2 学術総合センター12階</A>
  </DT>
		<DT>講師：河野健二 （慶大）</DT>
		<DT>定員：60名</DT>
	</DL>
    </LI>
    <LI>
	<DL>
		<DT>第2回：<A HREF="/archive/WS20240129_kimura.pdf" target=_blank>RISC-Vの最近動向 WorldGuard, IOMMUを中心に</A></DT>
		<DT>日時：2024年1月29日(月)13:30〜15:30</DT>
		<DT>共催：早稲田大学グリーン・コンピューティング・システム研究機構</DT>
		<DT>開催場所：<A href="https://www.waseda.jp/inst/gcs/access/" target="_new">早稲田大学グリーン・コンピューティング・システム研究開発センター (40号館) 1階プレゼンテーションルーム</A></DT>
		<DT>講師：木村啓二（早大）</DT>
		<DT>定員：60名</DT>
	</DL>
    </LI>
    <LI>
	<DL>
		<DT>第1回：<A HREF="./archive/WS20231218_suzaki.pdf" target=_blank>TEEの概要 RISC-V PMPを中心に</A></DT>
		<DT>日時：2023年12月18日(月)17:00〜19:00 (会場は20:00まで)</DT>
		<DT>開催場所：<A href="https://www.u-tokyo.ac.jp/campusmap/cam01_06_06_j.html">東京大学理学部7号館007号室(地下)(会場を変更しました)</A></DT>
		<DT>講師：須崎有康（情セ大）</DT>
		<DT>定員：50名</DT>
	</DL>
    </LI>
    </UL>

    <hr style="height:3px">
    <H4><p style="padding-bottom:0px">発起人</p></H4>
    <UL style="line-height:1.1">
      <li>代表：石川裕（NII/ROIS）</li>
      <li> システムソフトウェア：河野健二 （慶大）、光来健一（九工大）、須崎有康（情セ大）、合田憲人（NII/ROIS）、竹房あつ子（NII）</li>
      <li> アーキテクチャ：木村啓二（早大）、高前田伸也（東大）、塩谷 亮太（東大）、五島正裕（NII）</li>
    </UL>

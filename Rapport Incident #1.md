DDOS (Inondation ICMP)
Rapport d’Incident 
Modèle NIST


Scénario - Points importants
Incident : L’entreprise a subi une attaque par déni de service distribué (DDoS) de type inondation ICMP, qui a rendu le réseau interne inopérant pendant 2 heures. L'attaque a submergé le réseau, impactant les services critiques et causant une interruption du site web de l'entreprise.
Méthode d'attaque : Un flot massif de requêtes ICMP (ping) a été envoyé via un pare-feu mal configuré. Cette vulnérabilité a permis à l'attaquant d’inonder les serveurs, provoquant une saturation des ressources réseau.
Impact : Cette attaque a stoppé les services internes de l'entreprise, empêché l’accès des employés à leurs outils de travail et perturbé les services clients, affectant leur capacité à utiliser leurs propres sites web hébergés par l'entreprise.
Résolution initiale : L’équipe d’intervention en cybersécurité a mis en œuvre des actions correctives : blocage du trafic ICMP entrant, mise hors ligne des services non essentiels, et rétablissement des services critiques après l'identification de l'origine de l’attaque.
Identifier
Systèmes et actifs affectés :
Technologie : Pare-feu, serveurs internes, et réseau de l’entreprise ont été directement affectés.
Processus métier : L’attaque a causé une interruption complète des opérations de l'entreprise, affectant à la fois les processus internes et les services clients.
Personnes : Les employés de l’entreprise et les clients ont été impactés par l’incapacité à accéder aux systèmes hébergés, créant un arrêt temporaire des activités.


Protection
Mesures de protection mises en place :
Contrôle d'accès : Configuration des pare-feu pour filtrer et limiter le trafic ICMP non autorisé. Seuls les administrateurs réseau ont accès aux configurations critiques.
Sensibilisation/Formation : Formation supplémentaire pour l’équipe réseau afin de configurer correctement les règles de pare-feu et reconnaître les signes avant-coureurs d’attaques DDoS.
Sécurité des données : Bien que cette attaque n'ait pas directement compromis les données, des procédures ont été mises à jour pour améliorer la protection contre les futures attaques visant les données.
Technologie de protection : Mise en œuvre d’un système de prévention d’intrusion (IPS) et d'un pare-feu avec une limitation stricte du taux de paquets ICMP afin de prévenir les attaques similaires à l’avenir.

Détection (Detect)
Outils de détection des menaces :
Anomalies et événements : Un système de gestion des informations et des événements de sécurité (SIEM) a été déployé pour surveiller les comportements anormaux sur le réseau et alerter en temps réel sur les attaques potentielles.
Surveillance continue : Implémentation de processus de surveillance réseau continue via des systèmes IDS/IPS pour détecter les flux de trafic anormaux et bloquer automatiquement les attaques en cours.
Processus de détection : Le SIEM et les systèmes IDS permettent d'identifier des paquets suspects en temps réel, déclenchant des alertes dès qu’un comportement anormal est observé, notamment une inondation de trafic ICMP.
Réponse
Plan de réponse :
Planification de la réponse : L’équipe cybersécurité a immédiatement mis en œuvre une règle de pare-feu pour bloquer le trafic ICMP suspect et a pris des mesures pour isoler les serveurs affectés.
Communication : Les équipes internes ont été informées par le biais de réunions d’urgence et de communications écrites. Les clients ont été avertis de l'incident par email, avec un délai estimé de résolution.
Analyse : Une analyse post-incident a révélé la vulnérabilité dans la configuration du pare-feu, et des rapports d’activité réseau ont permis d’identifier l’origine du trafic malveillant.
Atténuation : Un processus d’isolation des serveurs touchés a été mis en place immédiatement pour contenir l'attaque, réduisant ainsi son impact global sur les services clients.
Améliorations : Un audit complet des configurations de pare-feu et des protocoles de réponse a été lancé afin d’améliorer la réactivité en cas d’attaque future. Des tests de résistance ont été programmés pour vérifier la robustesse du réseau.


Récupération
Plan de restauration :
Restauration des services : Les services ont été rétablis après la reconfiguration du pare-feu et la mise en œuvre de nouvelles règles pour limiter les paquets ICMP. Le réseau a été stabilisé en moins de 2 heures après l'attaque.
Améliorations continues : Des tests supplémentaires seront effectués pour vérifier la solidité des nouvelles règles de sécurité et la capacité de détection du système SIEM/IDS.
Communication : Une communication transparente a été établie avec les clients et les parties prenantes pour expliquer l'attaque, les actions correctives prises, et rassurer sur la sécurisation renforcée des systèmes.

Conclusion :
Grâce à la réactivité de l’équipe, l’entreprise a réussi à atténuer l’impact de l’attaque DDoS. Le renforcement des mesures de protection, la surveillance continue, et la mise en place d'un SIEM permettront de mieux anticiper et contrer ce type d'attaque à l'avenir.

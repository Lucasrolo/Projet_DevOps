pipeline {
    agent any
    
    parameters {
        string(name: 'CURRENT_DATE', defaultValue: '', description: 'Enter the current date (YYYY-MM-DD)')
    }
    
    stages {
        stage('Date Validation') {
            steps {
                script {
                    def date = params.CURRENT_DATE
                    echo "Current Date: ${date}"
                    
                    // Extract month and day from date
                    def (year, month, day) = date.split('-').collect { it.toInteger() }
                    echo "Processing notifications for Month ${month}, Day ${day}"
                }
            }
        }
        
        stage('January - Diary') {
            when { expression { return params.CURRENT_DATE.startsWith('2025-01') } }
            steps {
                script {
                    echo "=== January: Digital Diary Tracking ==="
                    sleep 2
                    
                    def (year, month, day) = params.CURRENT_DATE.split('-')
                    if (day.toInteger() <= 7) {
                        echo "First Week Goal: Make sure you have your journal ready!"
                        echo "Daily Task: Write in your diary about your thoughts and experiences."
                    }
                    
                    // Sunday evening check (assuming Sunday is day 7)
                    if (day.toInteger() % 7 == 0) {
                        echo "Weekly Sunday Reflection: How did this week go? Summarize your thoughts and goals!"
                    }
                }
            }
        }
        
        stage('February - Home Improvement') {
            when { expression { return params.CURRENT_DATE.startsWith('2025-02') } }
            steps {
                script {
                    echo "=== February: Home Redecoration Progress ==="
                    sleep 2
                    
                    def (year, month, day) = params.CURRENT_DATE.split('-')
                    if (day.toInteger() <= 15) {
                        echo "Reminder: Today is ${params.CURRENT_DATE}! Find a room or area you would like to change and think how you can improve it"
                    } else {
                        echo "Reminder: February is almost over! What's one last touch you can add to make your home feel more welcoming?"
                    }
                }
            }
        }
        
        stage('March - Self Care') {
            when { expression { return params.CURRENT_DATE.startsWith('2025-03') } }
            steps {
                script {
                    echo "=== March: Self-Care Journey ==="
                    sleep 2
                    
                    def (year, month, day) = params.CURRENT_DATE.split('-')
                    echo "Daily Reminder: Start your day right: Take a deep breath, stretch, and drink a glass of water!"
                    
                    if (day.toInteger() % 7 == 0) {
                        echo "Weekly Check-in: How did this week go? Try to improve and adjust your routine"
                    }
                }
            }
        }
        
        stage('April - Kindness') {
            when { expression { return params.CURRENT_DATE.startsWith('2025-04') } }
            steps {
                script {
                    echo "=== April: Daily Acts of Kindness ==="
                    sleep 2
                    
                    echo "Daily Reminder: Remember to perform an act of kindness today!"
                    
                    def (year, month, day) = params.CURRENT_DATE.split('-')
                    if (day.toInteger() % 7 == 0) {
                        echo """Weekly Kindness Suggestions:
                        1. Smile at three strangers
                        2. Write a thank-you note to someone who helped you recently
                        3. Offer help to someone who seems to need it"""
                    }
                }
            }
        }
        
        stage('May - New Experiences') {
            when { expression { return params.CURRENT_DATE.startsWith('2025-05') } }
            steps {
                script {
                    echo "=== May: Try Something New ==="
                    sleep 2
                    
                    def (year, month, day) = params.CURRENT_DATE.split('-')
                    if (day.toInteger() <= 10) {
                        echo "Have you started your new adventure yet? There's still time to be bold!"
                    }
                    
                    if (day.toInteger() % 7 == 0) {
                        echo """Weekly Activity Suggestions:
                        1. Try a new sport or exercise class
                        2. Learn a new skill online
                        3. Visit a place you've never been to"""
                    }
                }
            }
        }
        
        stage('June - Family Time') {
            when { expression { return params.CURRENT_DATE.startsWith('2025-06') } }
            steps {
                script {
                    echo "=== June: Family Connections ==="
                    sleep 2
                    
                    echo "Daily Reminder: Plan something special for your loved ones this weekend!"
                    
                    def (year, month, day) = params.CURRENT_DATE.split('-')
                    if (day.toInteger() % 7 == 0) {
                        echo """Weekly Family Activity Ideas:
                        1. Family dinner night
                        2. Weekend picnic
                        3. Game night or movie marathon"""
                    }
                }
            }
        }
        stage('July - Summer Festivals') {
            when { expression { return params.CURRENT_DATE.startsWith('2025-07') } }
            steps {
                script {
                    echo "=== July: Summer Festivals and Dancing ==="
                    sleep 2

                    def (year, month, day) = params.CURRENT_DATE.split('-')
                    echo "Daily Reminder: Enjoy summer festivals! Find a concert to attend, dance under the stars, and sing along to live hits."

                    if (day.toInteger() % 7 == 0) {
                        echo "Weekly Festival Reminder: Plan an evening with friends and enjoy the summer vibes!"
                    }
                }
            }
        }

        stage('August - Beach Night') {
            when { expression { return params.CURRENT_DATE.startsWith('2025-08') } }
            steps {
                script {
                    echo "=== August: Sleep a Night on the Beach ==="
                    sleep 2

                    def (year, month, day) = params.CURRENT_DATE.split('-')
                    echo "Daily Reminder: Plan a night on the beach. Take a blanket, enjoy the stars, and let the sunrise greet you."

                    if (day.toInteger() % 7 == 0) {
                        echo "Weekly Beach Night Tip: Don’t forget to take a night bath and fully enjoy the magical atmosphere."
                    }
                }
            }
        }

        stage('September - Discover the World') {
            when { expression { return params.CURRENT_DATE.startsWith('2025-09') } }
            steps {
                script {
                    echo "=== September: Explore New Horizons ==="
                    sleep 2

                    def (year, month, day) = params.CURRENT_DATE.split('-')
                    echo "Daily Reminder: Step out of your comfort zone and explore new places or hiking trails."

                    if (day.toInteger() % 7 == 0) {
                        echo "Weekly Adventure Reminder: Have you planned a hike or an adventure for this weekend?"
                    }
                }
            }
        }

        stage('October - Study') {
            when { expression { return params.CURRENT_DATE.startsWith('2025-10') } }
            steps {
                script {
                    echo "=== October: Learn Something New ==="
                    sleep 2

                    def (year, month, day) = params.CURRENT_DATE.split('-')
                    echo "Daily Reminder: Enroll in an online course or dive into a subject that fascinates you."

                    if (day.toInteger() % 7 == 0) {
                        echo "Weekly Learning Check: What new skill or knowledge have you gained this week?"
                    }
                }
            }
        }

        stage('November - Play an Instrument') {
            when { expression { return params.CURRENT_DATE.startsWith('2025-11') } }
            steps {
                script {
                    echo "=== November: Learn an Instrument ==="
                    sleep 2

                    def (year, month, day) = params.CURRENT_DATE.split('-')
                    echo "Daily Reminder: Practice your instrument and enjoy making music!"

                    if (day.toInteger() % 7 == 0) {
                        echo "Weekly Music Progress: Have you learned a new song or chord this week?"
                    }
                }
            }
        }

        stage('December - Conscious Breathing') {
            when { expression { return params.CURRENT_DATE.startsWith('2025-12') } }
            steps {
                script {
                    echo "=== December: Breathe Consciously ==="
                    sleep 2

                    def (year, month, day) = params.CURRENT_DATE.split('-')
                    echo "Daily Reminder: Take 5 minutes to focus on your breathing and ground yourself in the present moment."

                    if (day.toInteger() % 7 == 0) {
                        echo "Weekly Breathing Reflection: Are you feeling more grounded and present this week?"
                    }
                }
            }
        }
        
        stage('Notification Summary') {
            steps {
                script {
                    echo "=== Daily Resolution Summary ==="
                    echo "Date: ${params.CURRENT_DATE}"
                    
                    def (year, month, day) = params.CURRENT_DATE.split('-')
                    if (day.toInteger() <= 15) {
                        echo "Reminder: Time is running out to achieve your objectives for this month!"
                    } else {
                        echo "The end of the month is near—make sure to complete your objectives!"
                    }
                }
            }
        }
    }
    
    post {
        success {
            echo "Resolution tracking completed for ${params.CURRENT_DATE}"
        }
        failure {
            echo "Failed to process notifications for ${params.CURRENT_DATE}"
        }
    }
}

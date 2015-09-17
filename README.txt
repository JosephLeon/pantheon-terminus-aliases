# Pantheon and Terminus
alias term='terminus'
alias termsites='term sites show'
alias termlog='term auth log'
function termuli() {
  term drush uli --site=$1 --env=$2
}
function termenv() {
  term site environments --site=$1
}
function termcreateenv() {
  term site create-env --site=$1 --env=$2 --from-env=$3
}
function termdash() {
  term site dashboard --site=$1
}
function termcreate() {
  term site backups create --site=$1 --env=$2
}
function termget() {
  term site backups get --site=$1 --env=$2 --to-directory=$3
}
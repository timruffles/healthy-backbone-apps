
task :count do
	lines = `find manuscript  | grep .txt$ | while read f; do wc $f; done | awk '{ print $2 }'`
  puts lines.split("\n").map(&:to_i).inject(0, &:+)
end

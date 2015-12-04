# -*- coding: utf-8 -*-
require 'sinatra'
require 'pg'


# get '/' do
#   @res = res
#   erb :index
# end

get '/display' do
  conn = PGconn.connect("localhost", 5432, "", "", "tonetch", "tonetch", "")
  res = conn.exec("SELECT todo, line, expire FROM toDo ORDER BY line")
  @res = res
  erb :display
end


# if res
#   $res = res
#   # puts "<TABLE BORDER='1'>"
#   # puts "<TR><TH>ToDo</TH><TH>期限</TH><TH>超過日数</TH></TR>"
#   # res.each do |i|
#   #   puts "<TR>"
#   #   i.to_a.each do |e|
#   #     puts "<TD>#{e[1]}</TD>"
#   #   end
#   #   puts "</TR>"
#   # end
#   # puts "</TABLE>"
# else
#   puts "ToDoリストは空です．"
# end

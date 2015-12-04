# -*- coding: utf-8 -*-

# -*- coding: utf-8 -*-
require 'sinatra'
require 'pg'


# get '/' do
#   @res = res
#   erb :index
# end

get '/display' do
  conn = PGconn.connect('localhost', 5432, '', '', 'tonetch', 'tonetch', '')
  @conn = conn
  erb :display
end


post '/insert' do
  if params[:chkInsVal]
    conn = PGconn.connect('localhost', 5432, '', '', 'tonetch', 'tonetch', '')

    if res
      "hello"
    else
      "world"
    end

    @conn = conn
    @taskVal = params[:taskVal]
    @lineVal = params[:lineVal]
    erb :insertExec
  else
    erb :insValInput
  end
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
